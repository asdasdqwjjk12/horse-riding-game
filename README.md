# Unhackable — GitHub/jsDelivr package

## Upload and play
1. Create a PUBLIC GitHub repository, or use your existing public repository.
2. Unzip this package. Upload unhackable.8244c12ea161.svg to the repository root. Do not upload only the ZIP.
3. Commit the file to the main branch.
4. Replace YOUR-USERNAME and YOUR-REPO in this URL, then open it in a browser:

https://cdn.jsdelivr.net/gh/YOUR-USERNAME/YOUR-REPO@main/unhackable.8244c12ea161.svg#/

The SVG contains the compiled game, styles, horse and arena artwork.
It does not need a server, API, account, Node.js, or other game files.
Google Fonts is optional; the game uses system fonts if fonts are unavailable.
index.html is a standalone fallback for local use, GitHub Pages, or normal web hosting.
jsDelivr may serve HTML as text, so use the SVG URL for direct play through jsDelivr.

## Controls
Space, up arrow, W, click, or tap to jump. Jump at the green line.
Use LET'S RIDE to start and RIDE AGAIN to restart.
The personal best stays in browser storage when the browser permits it.

## Embedding
Use an iframe, not an img tag:
<iframe src="https://cdn.jsdelivr.net/gh/YOUR-USERNAME/YOUR-REPO@main/unhackable.8244c12ea161.svg#/" title="Unhackable horse jumping" width="100%" height="900" style="border:0"></iframe>

Scripts do not run when SVG is used as a regular image or in GitHub's image preview.
Open the CDN link directly or use an iframe.

## Updates and caching
The filename contains a content hash. A new export produces a new filename when the game changes.
Upload the new file and update your link. Keep older files if you still use their URLs.
For an immutable release, replace @main with a Git commit SHA or version tag.
The #/ suffix is optional for this game; it matches the example URL format.

## Security note
Unhackable is the game's name, not a security guarantee.
Public GitHub/CDN files and local scores can be inspected or changed by a visitor.
This export contains no credentials, backend endpoints, accounts, or private data.

## Rebuild in this workspace
pnpm --filter @workspace/horse-jumping run export:cdn
