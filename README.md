# RILUZO — Play Beyond Limits

RILUZO is a growing library of free, browser-based games. The project starts with **Perfect Timing**, a quick reflex arcade game, and is designed to make adding new games straightforward.

## Play locally

No build tools or package installation are required.

1. Download or clone this repository.
2. Open `index.html` in a modern browser.
3. Select **Perfect Timing** to play.

For a local web server, you can also run `python -m http.server 8000` from the repository folder and visit `http://localhost:8000`.

## Project structure

```text
riluzo/
├── index.html                 # RILUZO game library homepage
├── games/
│   └── perfect-timing/
│       └── index.html         # First playable game
├── assets/                    # Shared images, icons, and styles
├── README.md
└── LICENSE
```

## Add another game

1. Create a folder under `games/`, for example `games/snake/`.
2. Put that game's standalone `index.html` inside the folder.
3. Add a card to the games grid in the root `index.html`, linking to `games/snake/`.
4. Update the available-game count in the library homepage.

Keep each game self-contained where practical. Shared branding and reusable assets belong in `assets/`.

## Publish with GitHub Pages

1. Create a new **public** GitHub repository named `riluzo`.
2. Upload the contents of this folder to the repository root (not the enclosing folder).
3. In the repository, open **Settings → Pages**.
4. Under **Build and deployment**, choose **Deploy from a branch**.
5. Select the `main` branch and `/ (root)` folder, then save.
6. Wait for GitHub Pages to publish. The site URL will appear in the Pages settings.

When you are ready, add `riluzo.com` under the **Custom domain** section of Pages and configure the DNS records at your domain registrar as GitHub instructs. Enable HTTPS once it becomes available.

## Technology

- HTML
- CSS
- Vanilla JavaScript

There is no build step and no framework dependency in this starter version.

## License

See [LICENSE](LICENSE). If you later add third-party games, art, fonts, audio, or libraries, check their licenses and attribution requirements before publishing them here.
