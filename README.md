# Camera Object Detector - Modernized

This is a single-file web app that uses TensorFlow.js COCO-SSD to detect objects from your camera with a modern UI and production hardening.

Highlights:
- Lazy model loading (loads on Start for faster initial page load)
- Device selector (switch between cameras)
- Backend selector (webgl/wasm/cpu)
- FPS cap control (throttle detections for performance/battery)
- Class filter (show only specified classes)
- Snapshot capture (annotated PNG)
- Recording (annotated WebM via MediaRecorder)
- Auto-pause when tab hidden; resume on visible
- Settings persisted in localStorage
- PWA support (manifest + service worker)

Usage:
1. Serve over HTTPS or from localhost (e.g., `npx serve .`)
2. Open in Chrome/Firefox. Click Start, grant camera permission.
3. Try pressing `S` to start/stop quickly.

Notes:
- Icons `icon-192.png` and `icon-512.png` are referenced in the manifest. Provide your own or remove from manifest.
- MediaRecorder WebM codecs may vary by browser; VP9 is attempted with fallback to default if needed.

