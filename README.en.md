# Reading Companion

[简体中文](README.md) · [User guides](docs/USER_GUIDE.md) · [Downloads](https://github.com/xululu0401/reading-companion/releases/latest) · [Issues](https://github.com/xululu0401/reading-companion/issues)

Read local books or websites, take notes, and turn your ideas into image cards in one desktop workspace.

### [⬇ Download for macOS (Apple Silicon)](https://github.com/xululu0401/reading-companion/releases/download/v0.3.1/Reading-Companion-0.3.1-mac-arm64.zip)

Version **0.3.1** · ZIP installer · [Installation](#download-and-install) · [Release notes](https://github.com/xululu0401/reading-companion/releases/latest)

![Read and take notes side by side](screenshots/reading-notes.png)

Read on the left, write on the right, and adjust the split to fit your workflow.

## Download and install

Release `0.3.1` provides a ZIP for **macOS on Apple Silicon (M series)**. Intel Mac, Windows and Linux installers are not yet available. [Download the installer directly](https://github.com/xululu0401/reading-companion/releases/download/v0.3.1/Reading-Companion-0.3.1-mac-arm64.zip) without expanding the Release Assets list.

Extract and move 阅读搭子.app to Applications. This installer has **no official Developer ID signature or Apple notarization**, so macOS may block opening it. Keep system security protections enabled. Signing and notarization are planned for a future release. SHA256SUMS.txt verifies file integrity, not publisher identity. A separate mainland-China download endpoint is not configured yet.

## Features

- Local EPUB/PDF/TXT, bookmarks and reading progress; web reading works with an empty shelf.
- Browser navigation, saved pages and excerpts; custom website selections may need Copy then Paste as reading excerpt.
- Rich-text notes, images, simple sketches, local autosave, JSON backups and Markdown export.
- Bring-your-own-key AI providers, note summaries and share drafts.
- Image cards with covers and pagination; export PNG and captions for manual posting.
- Simplified/Traditional Chinese, English, Japanese and Spanish, with offline guides.

See the [English guide](docs/guides/en.md). Back up regularly: JSON backups exclude original books, website sessions and API keys. Deleting a shelf book also deletes its notes and share drafts after confirmation.

## Screenshots

### Turn notes into share cards

Edit text, choose a style, preview the result and export images.

![Share studio with live card preview](screenshots/share-studio.png)

### Help available offline

Built-in guides in five languages cover reading, notes, AI configuration, sharing and backups.

![Built-in offline user guide](screenshots/user-guide.png)

Screenshots show the actual desktop app with original demonstration text and notes.

## Current scope

No complete Goodnotes handwriting system, OCR, PDF annotation, book-wide search, cloud sync, automatic posting, managed AI, subscriptions, payments or automatic updates. Windows/Linux GUI and all real provider/site integrations have not been verified; translations need review. Basic features are free to use and will remain free. Optional paid features or services may be introduced in the future without requiring a purchase to keep using basic features. Third-party AI providers charge separately.

## License and privacy

See the [license](LICENSE) for software terms. You are welcome to share the official download link. Third-party components retain their own licenses; see [notices](THIRD_PARTY_NOTICES.md) and the Electron notices in the application. Reading Companion is independent of reading and social platforms.

Books and notes stay local by default. AI requests send the selected note text, title and book title only when requested. See [privacy](docs/PRIVACY.md) and [security reporting](SECURITY.md). Report bugs through Issues without credentials, personal notes or copyrighted books.
