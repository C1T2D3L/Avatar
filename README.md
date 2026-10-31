# Neels AI Avatar v0.3

## Fixes in this release
- Includes `avatar.glb` in the same folder as `index.html`.
- Fixes Three.js addon imports using an import map (the previous build could fail because OrbitControls/GLTFLoader could not resolve the bare `three` module).
- Loads the bundled GLB using a URL relative to the published page.
- Shows clearer loading/error status.
- Chat now responds locally to common avatar/project questions. This is a demo assistant, NOT a live AI model.

## Publish on GitHub Pages
Upload all four files to the repository root, preserving names: `index.html`, `avatar.glb`, `character-reference.png`, `README.md`. In Settings → Pages choose Deploy from a branch, branch `main`, folder `/ (root)`. Wait for deployment, then open the Pages URL in Chrome. Do not open `index.html` from the ZIP preview.

## Test
1. Confirm the top status changes to `3D MODEL LOADED`.
2. Drag on the model to orbit; pinch/scroll to zoom.
3. Send `hello`, `how do I rotate the model?`, or `what is next?` in chat.
4. If the model fails, the status panel now shows a diagnostic message.

## Still not implemented
A live AI model requires a backend service and private API credentials. Do not put secret keys in GitHub Pages/browser JavaScript. Full voice conversation, facial blendshape lip-sync, and Android overlay are later milestones.
