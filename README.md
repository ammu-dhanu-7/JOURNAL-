# Dear Diary — Premium PWA Starter

A responsive, installable diary and life-organizer web app. The main screen stays focused on the diary; the rest of the tools are hidden in the top-right menu.

## Features
- First-run 4-digit PIN setup and lock screen
- Diary home screen with 365 deterministic daily writing prompts
- Full-screen style editor: date, mood, title, writing, photo, sticker, voice note, page background and font controls
- 15 themes including cream, beige, charcoal, sage, rose, mocha and lavender
- Calendar with entry markers
- Habit tracker and custom tracker
- Bookshelf, daily/weekly/monthly task lists
- Dictionary / new words and cooking recipes / instructions
- Diary search and basic writing statistics
- JSON export/import backup
- PWA manifest, offline service worker and icon

## Run
Serve this folder from a local web server or HTTPS host. Some features (microphone, PWA installation and service worker) require HTTPS or localhost. The app may open directly as a basic page, but use a web server for full PWA behaviour.

## GitHub Pages
1. Create a GitHub repository.
2. Upload the contents of this folder to the repository root.
3. Go to Settings → Pages → Deploy from a branch → `main` → `/ (root)`.
4. Open the published HTTPS URL on Android Chrome.
5. Use Chrome's menu → Install app / Add to Home screen.

## Android APK
For an APK, package the hosted PWA with PWABuilder or a Trusted Web Activity workflow (Bubblewrap). Follow the tool's current signing instructions and keep your signing key private. An APK is not included in this ZIP.

## Data and security limitations — read before using
- This is a client-side starter, not an audited production application.
- Data is stored in browser localStorage on the current device. Browser/site data clearing, app removal, storage eviction or device loss can remove it. Export backups regularly.
- The PIN is a convenience gate only. It does not encrypt the data. Do not store highly sensitive or confidential information.
- There is no user account, cloud sync, server database, end-to-end encryption or automatic backup.
- Photos are limited to 3 MB each in the editor. Audio and images can still use substantial local storage.
- Voice recording requires browser microphone support and permission, and a secure context (HTTPS/localhost).
- Daily prompts are generated from a set of prompt phrases and rotate by calendar day; they are 365 day-indexed prompts, not 365 individually hand-written literary entries.
- Test thoroughly on your target Android device and browser before publishing or relying on the app.

## Files
- `index.html` — application UI and logic
- `manifest.webmanifest` — PWA metadata
- `sw.js` — offline cache
- `icon.svg` — app icon
