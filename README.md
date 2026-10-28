# Neels AI Avatar — v0.1 browser prototype

## What this version does
- Responsive browser-based 3D viewer using Three.js.
- Loads a local `.glb` or `.gltf` model in the browser.
- Supports orbit, zoom and camera reset.
- Shows the supplied 2D character reference until a real model is loaded.
- Includes a UI prototype for text chat, browser text-to-speech and optional speech recognition.

## What is not connected yet
- The uploaded photo is not a 3D model.
- AI chat is not connected to a language model.
- Voice is a browser demonstration only; there is no dedicated voice service or lip-sync yet.
- This is not yet an Android APK or floating overlay.

## Run it
Because the app uses JavaScript modules, open it from a local web server or host it as a static website (for example, GitHub Pages). Opening `index.html` directly as a file may block module imports.

1. Create a GitHub repository.
2. Upload `index.html`, `README.md`, and `character-reference.png` to the repository root.
3. In repository Settings, enable GitHub Pages from the main branch/root.
4. Open the Pages URL in a modern browser.
5. Use “Load 3D model (.glb/.gltf)” to load a rigged GLB model you own or are licensed to use.

## Next development step
Obtain/generate a photorealistic rigged human model as GLB. Prefer facial blendshapes/morph targets for future lip-sync. Then connect the AI service through a backend so secret API keys are never placed in browser code.
