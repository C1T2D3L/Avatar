# Neels AI Avatar — v0.2

This update bundles the uploaded GLB character model and attempts to load it automatically in the Three.js viewer.

## Files
- `index.html` — interactive browser viewer.
- `avatar.glb` — the supplied 3D model.
- `character-reference.png` — reference image fallback.
- `README.md` — setup instructions.

## Features
- Loads the bundled GLB model automatically when hosted from a web server.
- Orbit camera, zoom, and reset controls.
- Optional manual GLB/GLTF upload to test another model.
- Browser speech demo and local-only chat UI.

## Publish from a phone
1. Extract this ZIP.
2. Create a GitHub repository named `neels-ai-avatar`.
3. Upload all four files to the repository root (do not put them in a nested folder).
4. In repository Settings → Pages, publish from the main branch and root folder.
5. Open the GitHub Pages URL in Chrome. Allow a few seconds for the model and Three.js modules to load.

## Important limitations
- This is a browser prototype, not an Android APK.
- The GLB contains a skin/skeleton and an animation track, but detailed facial blendshapes/lip-sync and actual AI connectivity still need to be checked and integrated.
- Chat is not connected to an AI backend; voice uses browser features only.
- For an AI service, connect through a backend and do not put private API keys into `index.html`.

If the character appears too large or too small, the viewer's auto-fit can be tuned in `index.html`.
