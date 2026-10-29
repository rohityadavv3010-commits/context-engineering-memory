# Context hackathon website prototype

A responsive, single-page website for the **Why the Code Is Like This** repository-memory concept. It includes the product story, a sample Q&A demo, evidence details, visible uncertainty, and confirmation/review actions.

## Run locally

No build tools or package installs are needed.

1. Extract the source archive.
2. Open `index.html` in a modern browser.
3. Use one of the four sample prompts in the interactive demo.

If local-file restrictions prevent scripts from loading, serve this folder with Python:

```sh
python -m http.server 8000
```

Then visit `http://localhost:8000`.

## Source files

- `index.html` - page structure, navigation, demo, and evidence dialog
- `styles.css` - visual system and responsive layouts
- `data.js` - fictional demo questions and evidence
- `app.js` - question matching, evidence display, copy action, and local confirmation/review state

## Prototype scope

This is a front-end prototype. It does not connect to GitHub, GitLab, a live repository, an issue tracker, or an AI model. All records are fictional examples in `data.js`. Search selects the closest of four sample questions. Confirmation and review flags are stored in the current browser's local storage.

## Suggested next step

Connect a read-only repository integration and replace the fictional records with source IDs for real commits, reviews, issues, and documents. Preserve the distinction between recorded rationale, inference, and unresolved questions.
