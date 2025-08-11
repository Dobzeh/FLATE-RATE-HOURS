# Flat Rate Hours Tracker (PWA)

This repository contains a Progressive Web App (PWA) that helps dealership technicians track their flat‐rate hours. You can add, edit, import/export, and group entries by date. The application stores data locally in your browser and works offline thanks to its service worker and manifest file.

## Features

- **Add/Edit Entries**: Record RO number, tag, work performed, hours, pay type, service advisor, and notes.
- **Autosave**: Entries are saved to `localStorage` automatically whenever you add or update an entry.
- **Sorting & Filtering**: Click column headers to sort ascending/descending. Search across all fields with the search box.
- **Grouped View**: Toggle a grouped view that groups entries by date and shows daily totals. Click a date header to expand or collapse that day's details.
- **Import/Export CSV**: Bring in entries from a CSV with matching column headers or export your current entries as a CSV file.
- **Offline Support**: The included service worker caches core assets so you can continue to use the app when you have no network connection.

## Deploying on GitHub Pages

1. Create a new public repository on GitHub (e.g., `flat-rate-tracker`).
2. Upload all files in this folder (including the `icons` directory) to the root of your new repository. You can drag and drop them using GitHub's web interface.
3. Create an empty file named `.nojekyll` in the repository root. This bypasses Jekyll processing on GitHub Pages.
4. Commit your changes.
5. In your repository's **Settings** → **Pages**, set the source to **Deploy from a branch**, choose the `main` branch and the `/root` folder, then save.
6. After a minute or two, your app will be available at `https://YOUR_USERNAME.github.io/YOUR_REPO_NAME/`.

## Local Testing

If you'd like to test locally before deploying, you can serve the files with any static web server. For example:

```sh
python3 -m http.server 8000
```

Then visit `http://localhost:8000` in your browser.

Enjoy tracking your hours!