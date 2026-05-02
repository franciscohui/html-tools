# Goal
Create and deploy single page HTML tools

# Outcome
- Deploy two simple HTML tools to tools.partlysunnyai.com

# Approach
follow the same approach and guidelines from https://simonwillison.net/2025/Dec/10/html-tools/

# Steps

### Phase 2: Add AI tools

### Phase 1: setup and deploy initial tools; configure URL
- [x] Extract the page
- [x] Formulate instructions and guidelines and a reusable prompt
- [x] Initialize Git locally and connect to new GitHub Repo
- [x] Select 2 simple HTML tool ideas
- [x] Subagent 1: Scaffold, Test, and Commit Tool 1 (QR Code)
- [x] Subagent 2: Scaffold, Test, and Commit Tool 2 (Markdown Editor)
- [x] Deploy: Push to main and verify on default github.io URL
- [x] (Later) Configure tools.partlysunnyai.com custom domain

### Implemented Tools
- [x] **QR code creator** (`qr-code.html`): Type text/URL, generate a downloadable QR code.
- [x] **Markdown to HTML editor** (`markdown-editor.html`): Side-by-side live editor saving to localStorage.
- [x] **API Key Settings Page** (`settings.html`): Secure global setting management for LLM APIs.
- [x] **Groq Web Researcher** (`groq-researcher.html`): Agentic search using Groq Compound models.

### Standard HTML Tool Backlog
- **Base64 Image Encoder:** Drag and drop an image, get the data URI string (uses native FileReader API).
- **JSON Formatter/Validator:** Paste messy JSON, get it pretty-printed and validated.
- **CSS Box Shadow Generator:** Sliders to tweak a box shadow, provides the CSS output instantly.

### AI Tool Backlog (Phase 2)
*(These tools will require an LLM API key, managed via `settings.html` and stored in `localStorage`)*
- **Prompt Refiner:** Paste a rough prompt, and use an LLM (e.g., GPT-4o or Claude 3.5 Sonnet) to structure it, add constraints, and make it professional.
- **Tone Translator:** Paste an email or text, click buttons like "More Professional", "More Direct", "Kinder", and have the LLM rewrite it instantly.
- **Vision Alt-Text Generator:** Drag and drop an image (convert to base64 locally), send it to a Vision API, and generate descriptive alt-text for accessibility.
- **YouTube Transcript Summarizer:** Paste a raw YouTube transcript, and have the LLM generate a bulleted summary and extract key quotes.
- **JSON Data Extractor:** Paste unstructured text (like a messy email or article), and define a JSON schema. The LLM extracts the structured data and outputs clean JSON.
- **Groq Python Sandbox:** Utilizing the Groq `code_interpreter` tool to build an interface where the user types python code, and the LLM executes it securely and returns the output.
- **News Summarizer:** Uses Groq's `web_search` and `visit_website` to find the latest news on a user-provided topic and summarize it instantly.

---

### Scratch Area / Raw Ideas
*(Unpromoted ideas to brainstorm later)*
- simple API call
- simple image generation call
- upload a file, create a URL
- image or video generator
