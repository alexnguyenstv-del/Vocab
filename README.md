# Japanese Learning Hub — Fresh Build

A new static Japanese vocabulary and Kanji workspace. Built from scratch for GitHub Pages; no backend or build step is required.

## Run locally
Open `index.html` in a modern browser. Data is stored in that browser's LocalStorage.

## Deploy to GitHub Pages
1. Upload `index.html`, `styles.css`, `app.js`, and `README.md` to the repository root.
2. Open **Settings → Pages**.
3. Deploy from the `main` branch and `/ (root)`.

## Included in this first build
- Premium-style sidebar and dashboard.
- Vocabulary Inbox with seven-field paste import, preview, duplicate checks, editing and deletion.
- Vocabulary Boxes with multi-select membership management.
- Three typed vocabulary study modes and per-box/per-mode Need Review queues.
- Kanji Library, Kanji Boxes and typed Vietnamese-meaning study.
- Dictionary page with live autocomplete suggestions, a small offline starter set, save-to-Inbox/Box actions and Kanji saving.
- Kanji drawing canvas UI, ready for a future offline handwriting-recognition dataset.
- JSON backup export/import and local reset.

## Important scope notes
- The dictionary currently contains only a small starter set plus words in the user's Vocabulary Inbox. It is **not** a complete JMdict/KANJIDIC2 installation.
- The drawing canvas is implemented, but actual handwriting recognition is not yet connected because a licensed offline stroke-recognition dataset has not been bundled.
- Kanji metadata beyond the starter entries is marked `Needs verification`; do not treat missing readings or meanings as authoritative.
- Japanese IME input is supported through the operating system. The app guards Enter during IME composition, but actual conversion behavior depends on the browser and installed IME.
- Examples are required in the seven-field import format. Current format:

```text
Japanese | Hiragana | Romaji | English meaning | Vietnamese meaning | Part of speech | Example sentence(s)
私 | わたし | watashi | I; me | tôi | pronoun | 私は学生です。
```

## Data and privacy
- Learning data stays in this browser's LocalStorage unless the user exports it.
- Dictionary lookup is local and does not call a remote API.
- Export JSON periodically; clearing browser data can erase the local workspace.
