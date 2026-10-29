# Hóngmén 红门 — Mandarin Conversation Simulator

A single-page site where students practice realistic Mandarin conversations: an AI conversation partner, a character dictionary, and scenario challenges with goals and XP.

## Run it

Open `index.html` in a browser, or host it anywhere static (GitHub Pages, Netlify, Vercel). There is no build step.

## Note on the live AI partner

The AI replies use `window.claude` (Claude's artifact runtime), which is only present when the page is opened as a Claude artifact. On GitHub Pages or any other host the chat shows **Offline**; the dictionary, scenarios and layout still work.

To make the chat work on your own host, replace the `sample.json(...)` calls in `index.html` with a request to your own backend (for example a small serverless function that calls the Anthropic Messages API with your key). Never put an API key directly in the page.
