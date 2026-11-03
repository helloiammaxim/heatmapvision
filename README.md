# Heatmap Vision — Depth Tool

Browser tool that turns a webcam, video, image or depth sensor into a Z-depth map and colourises it with gradients. Open `index.html` over `https://` or `http://localhost` (cameras are blocked on some `file://` pages). No install needed.

## Sources
- **Webcam / image / video** — depth is estimated with Depth Anything V2 (Small or Base) running in the browser (WebGPU, falls back to WASM). Drag and drop files onto the view.
- **Depth sensor** — USB depth cameras such as Intel RealSense, Orbbec or Kinect-type devices in Chrome, read at full 16-bit precision with near/far range in metres.
- **Open depth map** — load an existing depth image or video (white = near), e.g. exported from iPhone LiDAR apps, and colourise it. iPhone LiDAR/Face ID and Windows Hello IR aren't accessible from browsers directly.

## Controls
- **View:** Gradient (with opacity over the source), Depth (grayscale), Source, Split wipe
- **Quality:** model size, model resolution (196–728 px), backend
- **Depth range:** auto range or locked range (no flicker on video), near/far clip, gamma, invert, temporal smoothing, edge softening
- **Stylize:** posterize steps, contour lines and opacity
- **Gradient:** presets (Thermal, Turbo, Inferno, Magma, Plasma, Viridis, Classic heat, Ice, Grayscale) and an editor — click the bar to add stops, drag to move, pick colours, delete, reverse
- **Export:** PNG of the current view, video recording (MP4 or WebM), and a 16-bit grayscale depth PNG for Blender displacement, Defocus or Mist

Settings are remembered between sessions.

## License

Free to use for personal and commercial work under the [PolyForm Shield License 1.0.0](LICENSE).

- ✅ Use the tool for free, for personal and client projects
- ✅ Everything you make with it (images and videos) is yours, including for commercial use
- ❌ Don't sell the tool, put it behind a paywall, host it as a paid service, or build it into a product that competes with it

© 2026 Max Soldatkin
