# BrahmaDeck Web Rewrite

Static browser rewrite of the original Python app.

## What changed
- No Tkinter UI
- No embedded PowerPoint preview
- Gemini calls use the official Google GenAI JavaScript SDK in the browser
- PPTX export uses PptxGenJS
- PDF export uses jsPDF
- Settings persist in localStorage

## Use
Upload `index.html` to itch.io as a static HTML project, or open it from any static host.

## Notes
- Enter your Gemini API key in the app.
- The browser SDK initialization is the same as the server-side SDK call, but Google documents warn not to expose API keys in production client-side code.
- The app uses structured outputs with JSON schema so the model returns predictable slide data.
