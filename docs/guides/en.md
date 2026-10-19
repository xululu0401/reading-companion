# Reading Companion user guide

For version 0.3.x. Read local books or websites, take notes, and make share cards in one workspace. An account or AI key is not required for basic use. This guide is available offline.

## 1. Get started

1. Open the desktop app. Choose “Open local file” for EPUB, PDF or TXT, or switch to “Browser reading” and enter a URL.
2. Select a book in the library and create a note on the right. Write a title and your thoughts.
3. Wait for “Saved locally”. This confirms a save on this device, not a cloud backup.
4. Choose “Create share cards”, edit the text and colors, then export images and copy the caption.
5. Use “Back up” and keep the JSON file somewhere you manage. Keep the original books separately.

Download installers from the official release page. Embedded websites and AI configuration require the desktop app.

## 2. Find your way and view all notes

- The library contains books and reading links. Search finds saved book titles and note titles/body text, not the full text of original books.
- Drag the divider between reading and notes to resize. Double-click to reset; focus it and use arrow keys for small adjustments.
- Open the dropdown beside the current note title to see all notes for the selected book. “Notes: 4” counts regular notes, excerpts and summaries; the number itself is not the list button.
- “Read & write” and “Share studio” switch workspaces while keeping the reading page loaded. Changing books or explicitly refreshing may navigate away.
- Use “Read fullscreen”, then the exit button or Esc to return. “Focus on writing” expands the note area; its restore button returns to the normal layout.
- The question-mark button in the top bar opens this guide without navigating away from your reading page.

Deleting books: click the trash button beside a book in the left shelf, or choose “Remove from shelf” when editing its details. The confirmation shows the number of associated notes and offers a backup action. Confirming also deletes that book’s notes, excerpts, summaries and share drafts; this cannot be undone. Original files on your computer and books in website accounts are unaffected; imported file caches remain in the app. You can delete the last book and then add a URL or open a file from the empty shelf.

## 3. Local EPUB, PDF and TXT

Choose “Open local file”. The file limit is 50 MB, or 10 MB for TXT. DRM-protected books are unsupported. Imported files stay on this device.

- EPUB: use contents, previous/next chapter, font size, themes and chapter bookmarks. Reading position is saved. The reader uses its own layout and does not fully reproduce publisher styles, fonts or fixed layouts.
- PDF: jump to pages, zoom and add page bookmarks. Text selection needs a text layer; scanned pages cannot be excerpted directly. OCR, handwritten PDF annotations and interactive forms are not available.
- TXT: use UTF-8 or BOM-marked UTF-16. The reader creates sections and supports size, themes and bookmarks. Re-save garbled files as UTF-8 before importing.

If an original file is missing, open the exact same file again to associate it with existing notes and progress by fingerprint. Changed bytes may identify a different book. Keep independent copies of original files.

## 4. Browser reading and web excerpts

Enter a URL such as `https://weread.qq.com` directly and press Enter, or choose a reading shortcut. Ordinary keywords are sent to Baidu search; recognized reading-service names can open their site directly. Log in using the website’s own flow. Use back, forward and refresh/stop for navigation; save the current page to your library with the reading-entry control.

Ordinary new-window links open in the reading pane by default. Login, payment or explicitly requested popup flows may open separately. “Allow separate windows” changes the handling of ordinary site popups.

For standard text, select it and right-click to save a reading excerpt. Check the text, source and destination book in the confirmation dialog.

Some sites, including WeRead, draw custom text selections. Use the site’s “Copy” action first, then the app’s right-click “Paste as reading excerpt”. The clipboard is read only after that action. Check that it contains the intended text. You can also open “Excerpt” on the right and paste manually with a source.

Website subscriptions, login and highlighting belong to the website. The app does not bypass membership, copy restrictions or DRM, and not all sites permit embedding. If a page fails, check the same site in a normal browser.

## 5. Excerpts, notes and autosave

Regular notes hold your own thoughts. Excerpts preserve source text with a chapter, page or URL. AI summaries are saved as separate notes. All three appear in the selected book’s note list and can be edited or shared.

For local excerpts, select text entirely inside the reading pane and right-click, or use “Save selected text as excerpt”. The confirmation dialog supports manual text up to 20,000 characters.

The editor supports headings, bold, italic, lists, quotations, images, simple sketches, undo and redo. Sketches are illustrations, not a full handwriting notebook or recognition system. Note images do not automatically become share-card covers.

Notes and share drafts save automatically. Watch “Saving”, “Saved locally” or “Save failed”. If saving fails, export a backup first and then retry; do not clear app data. “Save settings” in AI configuration only saves service settings. The note’s download button exports Markdown for text reuse, not a complete backup. Deleting a note also deletes its share draft; there is no recycle bin, so back up first if needed.

## 6. Set up AI services

AI is optional. You provide your own key and pay the chosen provider. Official managed AI, subscriptions and top-ups are not implemented.

1. Open “Settings & AI”, choose a provider preset and “Add configuration”. Presets include DeepSeek, OpenAI, Claude, Gemini, Qwen, Kimi, GLM, Ollama and Custom API.
2. Enter a name, API type, URL and key. Names help distinguish personal, work and local configurations.
3. “Fetch models” and choose one, or enter the provider’s model ID manually. A URL and key do not guarantee automatic model discovery.
4. “Test connection” sends a short prompt without notes and may incur a small charge. Fetching models also sends authentication to the configured endpoint.
5. “Save and activate”; check the active-service label. To switch, select another profile and save and activate it. “Save settings” saves edits; the first saved profile becomes the default. Up to 30 profiles can be saved.

Supported protocols: OpenAI Chat Completions, OpenAI Responses and Anthropic Messages. Gemini uses its OpenAI-compatible endpoint. Include the provider’s required version path, such as `https://api.example.com/v1`; `/v1` is not added automatically. Remote URLs need HTTPS; local loopback services can use HTTP. Credentials, query parameters and fragments are not allowed in the URL.

For Ollama, install and start it separately and prepare a model first. The usual URL is `http://localhost:11434/v1`; the key can be blank. Fetch models or enter an installed model name. This app does not install or download models.

Saved keys are encrypted by the operating system and are not shown again. Leave the key field blank to keep an existing key. Changing the URL or protocol requires re-entering the key or explicitly removing it. Deleting the active profile leaves no active service until you enable another one.

## 7. Summarize and polish with AI

Select a note, open its AI organizer and choose “Generate”. Input must contain at least 10 characters and at most 50,000. Only that note’s text, title and book title are sent, not the original book, other notes, cookies, images or sketches.

The generation dialog captures a snapshot when opened. Edits made while generation is running are not added to that request. Finish the current request and reopen generation to use the latest note.

Edit and verify the result, then save it as a new summary note; the original remains. “Polish with AI” in the share studio prepares a title, body and hashtags for the share draft. Apply the result only after reviewing quotations and claims. Regeneration sends another potentially billable request.

## 8. Share cards and synchronization

1. Select a note and open “Create share cards” or “Share studio”.
2. Edit title and body, choose colors and optionally add a JPG, PNG or WebP cover. Preview updates after a short rendering delay.
3. Long text is paginated. Browse pages with the arrows; cards are 1080 × 1440 pixels, in a 3:4 ratio.
4. “Export current card” saves one PNG. Export each page separately; batch export is not implemented.
5. Copy the caption, then upload the images and text to Xiaohongshu or another platform yourself. The app does not post automatically.

Title and body initially follow the note. Editing either field in the share studio makes that field independent, so later note changes will not overwrite it. Use the title/body reset controls or reset both to follow the note again. This replaces the independent text with the current note, so preserve any edits you need first. Colors and cover are retained.

## 9. Back up, restore and change computers

Autosave is local. Export JSON backups regularly and keep original books separately. JSON is structured restore data, not an image for sharing, and need not be edited by hand.

Backups include book metadata, fingerprints, reading progress, bookmarks, notes, note images and share drafts. They exclude original books, website cookies, API keys and language preference. Backup files are not additionally encrypted.

To move computers: export the latest JSON → copy original books separately → open the app on the new computer → back up any existing notes there → choose “Restore” and review the counts → confirm → reopen the identical original files → log in to websites and configure AI/language again.

Restoring replaces the current library and notes; it does not merge libraries. Backup files must be under 100 MB. Notes remain usable without the original books, but the book contents cannot be recovered from JSON. Browser preview and desktop storage are separate; use JSON to transfer notes between them.

## 10. Languages, privacy and local data

“Settings & AI → Interface language” supports Simplified Chinese, Traditional Chinese, English, Japanese and Spanish, with a system-language option. Changes apply and save immediately, independently of AI settings. Unsupported system languages fall back to English. Existing notes, book titles and websites are not translated.

This guide follows the interface language; its own language selector changes only the guide. All guide content is bundled offline. AI requests ask for the current interface language, but actual results depend on the model.

There is no default cloud sync, telemetry or advertising SDK. Books, notes, website sessions and AI settings are separate. Local notes are not an encrypted vault. Do not casually clear app or browser site data.

Default desktop user-data folder: `~/Library/Application Support/reading-companion` on macOS, usually `%APPDATA%/reading-companion` on Windows, and `$XDG_CONFIG_HOME/reading-companion` or `~/.config/reading-companion` on Linux. Quit and back up before troubleshooting these files; do not edit live data manually. See the repository privacy and security documents for details.

## 11. Troubleshooting

- Can’t see all notes? Select the book and open the dropdown next to the current note title.
- Empty excerpt? Select within the reading text. For custom website selections, copy through the site and paste as an excerpt. Scanned PDFs need an external OCR tool.
- Share preview not following edits? Check whether the affected field is independent; restore following if needed and wait for rendering. Add a cover separately.
- Wrong interface language? Check for a manual override in settings. Website text and operating-system dialogs use their own language.
- AI 401/403: check key and account/model permissions. 404: check version path, protocol and model ID. 429: check quota or rate limits. Timeout: check network and provider status.
- Model listing unsupported? Enter a valid model ID manually and test; listing failure does not necessarily prevent generation.
- Secure storage unavailable? Check the OS keychain/credential service. Keys cannot be saved using Linux’s plain-text backend.
- Slow refresh or login page? Refresh requests the website again. Check network, website and login session. Switching to share mode should not refresh reading; report reproducible failures.
- Save/load failure? Preserve existing data, export what you can or use a known backup. Do not delete the data directory as an experiment.

## 12. Limitations and feedback

OCR, handwriting recognition, PDF annotation, original-book full-text search, cloud sync, automatic social posting and official managed AI are not available. It does not offer the complete Goodnotes feature set. Windows/Linux GUI, every site and every model have not been fully tested. Translations still need native-speaker review.

Report the app version, OS and architecture, language, desktop/preview mode, exact steps, expected and actual behavior, and a screenshot without private data. Prefer a small original test file; never attach real keys, cookies, copyrighted books or your whole note library.

Report ordinary bugs at https://github.com/xululu0401/reading-companion/issues . For security issues, follow SECURITY.md in the public repository and use a private channel; do not disclose sensitive details publicly.
