# Akay Game Dev — Website

This repository hosts a simple personal website for Akay's game development progress. The site files (index.html, privacy.md) are placed at the repository root so GitHub Pages can serve them from the main branch.

Deployment notes:
- The site expects a Unity WebGL build folder named `Build/` at the repository root. If you have exported a WebGL build from Unity, place the entire Build folder (including index.html, .data, .wasm, .js, and any TemplateData) in the repository root.

Troubleshooting:
- If the embedded build does not load, open the browser console to check for 404 or MIME type errors — these usually indicate missing files or incorrect paths.
- Make sure the Build folder contains the same relative paths as produced by Unity.
