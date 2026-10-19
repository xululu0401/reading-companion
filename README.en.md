# Reading Companion

[简体中文](README.md) · [User guides](docs/USER_GUIDE.md) · [Downloads](https://github.com/xululu0401/reading-companion/releases) · [Issues](https://github.com/xululu0401/reading-companion/issues)

Read local books or websites, take notes, and turn your ideas into image cards in one desktop workspace.

**Proprietary software; the current preview is free to use.** This repository contains product documentation and downloads, not the application's implementation source. It is independent of reading and social platforms.

## Download

Release `0.3.1-beta.1` provides a ZIP for **macOS on Apple Silicon (M series)**. Intel Mac, Windows and Linux installers are not yet available. Download the `mac-arm64` ZIP from [Releases](https://github.com/xululu0401/reading-companion/releases); GitHub's automatic “Source code” archives contain these public documents only.

Extract and move 阅读搭子.app to Applications. This preview has **no official Developer ID signature or Apple notarization**, so macOS may block opening it. Do not disable system security protections; wait for a signed release if you need normal installation. SHA256SUMS.txt verifies file integrity, not publisher identity. A separate mainland-China download endpoint is not configured yet.

## Features

- Local EPUB/PDF/TXT, bookmarks and reading progress; web reading works with an empty shelf.
- Browser navigation, saved pages and excerpts; custom website selections may need Copy then Paste as reading excerpt.
- Rich-text notes, images, simple sketches, local autosave, JSON backups and Markdown export.
- Bring-your-own-key AI providers, note summaries and share drafts.
- Image cards with covers and pagination; export PNG and captions for manual posting.
- Simplified/Traditional Chinese, English, Japanese and Spanish, with offline guides.

See the [English guide](docs/guides/en.md). Back up regularly: JSON backups exclude original books, website sessions and API keys. Deleting a shelf book also deletes its notes and share drafts after confirmation.

## Preview limits

No complete Goodnotes handwriting system, OCR, PDF annotation, book-wide search, cloud sync, automatic posting, managed AI, subscriptions, payments or automatic updates. Windows/Linux GUI and all real provider/site integrations have not been verified; translations need review. The app is free for this release; third-party AI services may charge separately. Future paid features will have separately disclosed terms.

## License and privacy

Install and use this release under the [proprietary license](LICENSE). Permission to reuse the proprietary implementation, modify, redistribute or resell it is not granted except as permitted by law. Share the official download link instead. Third-party components retain their own licenses; see [notices](THIRD_PARTY_NOTICES.md) and the Electron notices in the application.

Books and notes stay local by default. AI requests send the selected note text, title and book title only when requested. See [privacy](docs/PRIVACY.md) and [security reporting](SECURITY.md). Report bugs through Issues without credentials, personal notes or copyrighted books.
