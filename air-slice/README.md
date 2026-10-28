# Air Slice v1.0

A new fingertip-controlled arcade game based on the successful Gesture Catch MediaPipe deployment.

## Install (IMPORTANT)

Your GitHub Pages repository should be arranged as:

```
gesture-catch/
  index.html                # existing Gesture Catch — keep unchanged
  vendor/                   # existing locally hosted MediaPipe assets
    vision_bundle.mjs
    wasm/...
  models/
    hand_landmarker.task
  air-slice/
    index.html              # this new game
```

Upload the **air-slice folder** to the root of the EXISTING repository. Do not overwrite its root index.html. You do NOT need to download MediaPipe again.

Open https://sindooratm1990.github.io/gesture-catch/air-slice/?v=1

## Controls
- Hold your index finger in view of the tablet's front camera, then move it quickly across flying fruit.
- Hold a closed fist for several frames to pause; open palm to resume.
- Drag a finger on the touchscreen to test slicing without the camera.
- New game resets the score.

## Notes
- GPU is selected by default based on earlier Lenovo Tab Plus benchmarking; CPU can be selected before starting the camera.
- The AI model and runtime are loaded from `../vendor/` and `../models/`.
- The TV simply mirrors the tablet; use landscape orientation.
- This is an original fruit-slicing prototype, not the commercial Fruit Ninja game.
