# Goal
Create and deploy single page HTML tools

# Outcome
- Deploy two simple HTML tools to tools.partlysunnyai.com

# Approach
follow the same approach and guidelines from https://simonwillison.net/2025/Dec/10/html-tools/

### Steps
- [x] Extract the page
- [x] Formulate instructions and guidelines and a reusable prompt
- [ ] Initialize Git locally and connect to new GitHub Repo
- [ ] Select 2 simple HTML tool ideas
- [ ] Subagent 1: Scaffold, Test, and Commit Tool 1
- [ ] Subagent 2: Scaffold, Test, and Commit Tool 2
- [ ] Deploy: Push to main and verify on default github.io URL
- [ ] (Later) Configure tools.partlysunnyai.com custom domain

### Ideas for tools
- **QR code creator:** Type text/URL, generate a downloadable QR code (using a CDN library like qrcode.js).
- **Markdown to HTML editor:** Side-by-side markdown editor using marked.js, saves to localStorage.
- **Base64 Image Encoder:** Drag and drop an image, get the data URI string (uses native FileReader API).
- **JSON Formatter/Validator:** Paste messy JSON, get it pretty-printed and validated.
- **CSS Box Shadow Generator:** Sliders to tweak a box shadow, provides the CSS output instantly.
- simple API call
- simple image generation call
- upload a file, create a URL 
- youtube transcript generator + summarizer
- idea refiner: start with prompt, system improves
- translator
- image or video generator
- image descriptor
