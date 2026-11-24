# AZISLY CRM

A static, single-user EdTech sales CRM built with HTML, CSS, vanilla JavaScript and IndexedDB. It is designed for GitHub Pages and does not need a server or build step.

## Run locally

Open the folder with a static server (for example VS Code Live Server) and open `index.html`. Modern browsers require HTTP(S), rather than `file://`, for reliable module and IndexedDB behaviour.

## Data and backups

All records live in this browser's IndexedDB database (`azislyCRM`). Data remains after refresh, but can be lost if site data is cleared. Use **Settings → Export complete backup** regularly. Import validates the backup schema and asks before replacing records.

The Settings page can add fictional demo data, export CSV files, configure future course prices, and reset local data.

## GitHub Pages deployment

1. Create a GitHub repository and upload this project’s files.
2. In the repository, open **Settings → Pages**.
3. Under **Build and deployment**, choose **Deploy from a branch**.
4. Select `main` (or your deployment branch), folder `/ (root)`, then save.
5. Open the URL GitHub supplies after deployment finishes.

All internal assets use relative paths, so the site works from a repository subdirectory. Browser data is local to each device/browser and is not synchronized or encrypted by this application.
