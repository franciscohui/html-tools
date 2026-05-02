# HTML Tool Creation Guidelines for Agents

This document outlines the principles, guidelines, and deployment instructions for creating self-contained HTML tools. Any agent tasked with building a new HTML tool should read and adhere to these rules.

## Core Principles & Guidelines

When building an HTML tool, follow these architectural constraints to ensure the tool is highly portable, easy to prompt, and simple to host:

1. **Single File Architecture:** Combine all HTML, JavaScript, and CSS into a single `.html` file. This minimizes hosting friction and makes it trivial to copy/paste code between LLMs and editors.
2. **Zero Build Step (No React):** Avoid frameworks that require a compilation or build step (like React/JSX, Vue SFCs, or Angular). Use vanilla HTML, CSS, and JavaScript. 
3. **Use CDNs for Dependencies:** If you need an external library (e.g., `PDF.js`, `Tesseract.js`, `Pyodide`, formatting libraries), load it directly from a trusted CDN (like cdnjs, jsDelivr, or unpkg). Never use `npm install` or local `node_modules` for these tools.
4. **Keep it Small and Maintainable:** Aim for a few hundred lines of code. If a tool becomes too complex, consider if it can be broken down. Small tools are easier for LLMs to read, understand, and completely rewrite if necessary.
5. **Leverage the Clipboard:** Utilize JavaScript clipboard events for rich copy-and-paste interactions. Tools that accept pasted content, transform it, and copy it back to the clipboard provide excellent user experiences.
6. **State Management:**
   - **URL State:** Persist small configuration state or user input in the URL (e.g., using the URL hash) so the tool's current state can be easily bookmarked or shared.
   - **LocalStorage:** For larger state, or sensitive information like API keys, use the browser's `localStorage` API. **Never hardcode API keys or secrets in the HTML file.** If an LLM API is needed, prompt the user for their key and save it to `localStorage`.
7. **Utilize CORS-Enabled APIs:** Fetch data directly from the browser using APIs that support Cross-Origin Resource Sharing (CORS), such as GitHub (via `raw.githubusercontent.com`), PyPI, Bluesky, Mastodon, etc.
8. **Local File Processing:** Use `<input type="file">` to let users process files locally in their browser. You do not need a backend server to read, parse, or modify files.
9. **Client-Side Downloads:** If the tool transforms data, provide a way for the user to download the result directly from the browser by dynamically generating file blobs.
10. **Embrace WebAssembly (WASM):** For heavy computational tasks (like OCR, video processing, or running Python/SQLite), load WASM modules or environments like Pyodide directly from CDNs.
11. **Consistent Footer:** Always include a small footer at the bottom of the tool that links back to the main repository: `Built with the <a href="https://github.com/franciscohui/html-tools">HTML Tools pattern</a>`.

---

## Reusable Base Prompt

When spinning up a subagent or asking an LLM to generate the initial prototype, use this base prompt template:

```text
Build a single-file HTML application that [INSERT TASK/IDEA DESCRIPTION HERE]. 

Follow these strict constraints:
- Use inline JavaScript and CSS within the single HTML file.
- Do NOT use React or any framework that requires a build step. Use vanilla JS/DOM manipulation.
- Load any necessary external dependencies directly from a public CDN (cdnjs, jsdelivr).
- Make the UI look modern, clean, and responsive (use native CSS or a lightweight CDN CSS framework if necessary).
- [Optional depending on tool] Persist the user's input/state in the URL hash so it can be shared.
- [Optional depending on tool] If an API key is required, prompt the user for it and securely store it in localStorage.
- Always include a footer: `Built with the <a href="https://github.com/franciscohui/html-tools">HTML Tools pattern</a>`.
- The final output must be entirely self-contained in one file.
```

---

## Workflow & Deployment Instructions

To take an idea from concept to production with minimal human intervention, follow this workflow:

### 1. Local Creation
1. Define the specific functionality and write a targeted prompt using the template above.
2. Generate the single `.html` file.
3. Save the file locally in the workspace (e.g., `tool-name.html`).

### 2. Local Testing
1. Because the tool is a single file with no build step, you can often test it simply by opening the file URL in a browser (`file:///path/to/tool-name.html`).
2. If the tool fetches external APIs or uses certain web worker features, it may require an HTTP server due to CORS/file protocol restrictions. In that case, spin up a quick local server in the directory:
   ```bash
   python3 -m http.server 8000
   ```
   (Then access via `http://localhost:8000/tool-name.html`)

### 3. Automated Deployment (GitHub Pages)
Because there is no build step, deployment is instantaneous and can be fully automated:
1. Ensure the workspace is initialized as a Git repository.
2. Add the new `.html` file to the repository.
   ```bash
   git add tool-name.html
   git commit -m "Add tool-name HTML tool"
   ```
3. Push to the remote repository.
   ```bash
   git push origin main
   ```
4. **Prerequisite:** The target repository must have GitHub Pages enabled (e.g., pointing to the `main` branch root). Once pushed, the tool is immediately live at `https://[username].github.io/[repo]/tool-name.html`. No CI/CD configuration is required.
