# 3D Character Demo with model-viewer

Self-contained example of an interactive 3D viewer for the web, using the
[`<model-viewer>`](https://modelviewer.dev) component (Google, WebGL/glTF)
with an animated character.

## What's included

- A single HTML file with no external dependencies: the `model-viewer`
  library and the 3D model are embedded directly in the file (the model
  as a base64 `data:` URI).
- Sample model: **RobotExpressive.glb** (CC0 license), with 13 different
  animations (Idle, Walking, Running, Dance, Jump, Yes, No, Wave, Punch,
  ThumbsUp, Sitting, Standing, Death).
- Basic controls: mouse/touch rotation, auto-rotate, buttons to switch
  animations, and a loop toggle.

## How to use it

1. Download or clone this repository.
2. Open `personaje-3d-demo.html` directly in your browser (double-click
   or drag it into a tab). No server or internet connection required.

## How to swap the character

1. Get a free `.glb` model, for example from [Sketchfab](https://sketchfab.com)
   (filter by CC0 or CC-BY license) or the
   [Khronos sample assets gallery](https://github.com/KhronosGroup/glTF-Sample-Assets).
2. Convert the file to base64 and replace the `src` attribute of the
   `<model-viewer>` element (or just point `src` to a public URL of the
   model if you don't need the HTML to be fully offline).
3. Update the list of animation names in the script to match the ones
   in the new model.

## Tech

- [`@google/model-viewer`](https://github.com/google/model-viewer)
  (Apache-2.0) — a web component built on Three.js/WebGL for displaying
  and interacting with 3D models, with built-in AR support.
- [glTF/GLB](https://www.khronos.org/gltf/) format, the open standard
  for 3D models on the web.

## License

This example project is free to use. The `RobotExpressive.glb` model is
licensed under CC0. The `model-viewer` library is licensed under
Apache-2.0.
