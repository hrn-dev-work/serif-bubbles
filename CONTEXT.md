# Context

Single-file browser tool. Open `index.html`. No server, no account, no environment secrets.

It draws speech-bubble PNGs for note articles. The right speaker defaults to わたし (white, green border) and the left speaker defaults to メェ助 (cream, gold border). Both display names can be changed. Width is 800px. Dialogue text is 30px. One line is at most 80 characters.

Icons, lines, and export preferences stay in `localStorage`. A failed write still leaves the in-memory session usable. The page must not send the script or icons anywhere (`connect-src 'none'`).

Human docs: `README.md` (Japanese), `README.en.md`, `docs/ja/`, `docs/en/`.

Security notes: `docs/agents/security.md`.
