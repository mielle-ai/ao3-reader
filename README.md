# mielle v2 — iPhone EPUB reader

## Install on iPhone

**Important:** The ZIP itself is not an installable iPhone app. Opening `index.html` from Files does not provide a reliable persistent library. The site must be hosted at an HTTPS address.

1. Unzip `mielle-reader-v2.zip` on a computer.
2. Create a public GitHub repository, such as `mielle-reader`.
3. Upload all **five** files from the `mielle-reader-v2` folder into the repository root: `index.html`, `jszip.min.js`, `sw.js`, `manifest.webmanifest`, `icon.svg`.
4. In GitHub: **Settings → Pages → Deploy from a branch → main / (root) → Save**.
5. Wait for the Pages URL to appear, then open it in **Safari** on your iPhone.
6. Tap **Share → Add to Home Screen → Add**.
7. Launch mielle from your home screen. Tap **Try sample story** to check the reader.
8. On AO3, download a work as **EPUB**, save it in Files, and tap **Import EPUB** in mielle.

## Features

- Local EPUB import and personal library (IndexedDB)
- Search titles/authors
- Chapter selection and next/previous chapter
- Saved chapter, scroll position, and reading percentage
- Bookmarks (tap star to save; double-tap star to return to saved bookmark)
- Four themes and three font options; font size controls
- Bundled ZIP parser: no external CDN dependency
- Offline app shell after first successful HTTPS load

## Limitations

- This is a web app, not a signed native iOS `.ipa`.
- It does not sign into AO3, browse AO3 internally, or sync your AO3 account.
- EPUBs with elaborate layouts, embedded fonts, DRM, or unusual formatting may not display perfectly.
- Books and progress stay on this device and origin. Keep EPUB backups in Files/iCloud Drive.
- Clearing Safari site data or switching to a different hosting domain can erase or separate the library.
- Safari may reclaim stored data under storage pressure.
