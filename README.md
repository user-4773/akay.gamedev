# Akay Game Dev — Website

This repository hosts a simple personal website for Akay's game development progress. The site files (index.html, privacy.md) are placed at the repository root so GitHub Pages can serve them from the main branch.

Deployment notes:
- The site expects a Unity WebGL build folder named `Build/` at the repository root. If you have exported a WebGL build from Unity, place the entire Build folder (including index.html, .data, .wasm, .js, and any TemplateData) in the repository root.
- An empty file named `.nojekyll` is included to ensure GitHub Pages serves build files without Jekyll filtering.
- To enable Pages: go to the repository Settings → Pages, and select the `main` branch and the `/(root)` folder. Save and wait a few minutes for the site to publish.

Troubleshooting:
- If the embedded build does not load, open the browser console to check for 404 or MIME type errors — these usually indicate missing files or incorrect paths.
- Make sure the Build folder contains the same relative paths as produced by Unity.
- **Brotli Compression Issues**: If you see MIME type errors for `.br` files on GitHub Pages, you may need to rebuild your Unity project with "Compression Format" set to "Gzip" or "Disabled" instead of "Brotli" in Unity's Project Settings → Player → Publishing Settings. GitHub Pages may not properly serve Brotli-compressed files without custom server configuration.

If you want, I can instead move the site files into a /docs folder and configure Pages to serve from `docs/`.