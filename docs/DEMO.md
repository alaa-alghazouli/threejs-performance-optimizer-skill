# Demo Walkthrough

This repository ships a skill package, not a web app. The fastest way to see value is with realistic prompt walkthroughs.

## Demo 1: Draw-call bottleneck

### Prompt

"My Three.js scene drops to 24 FPS when orbiting. Please profile likely bottlenecks, reduce draw calls, and preserve visual quality."

### Expected skill behavior

- Requests or inspects baseline metrics (`renderer.info`, FPS, profiler).
- Identifies draw-call pressure and scene graph churn.
- Recommends or applies:
  - `InstancedMesh` for repeated objects
  - static geometry merges where interactivity is not required
  - material reuse and variant reduction
- Returns before/after metrics and tradeoffs.

## Demo 2: R3F state-induced jank

### Prompt

"In React Three Fiber, pointer interactions are janky. Optimize frame-loop patterns."

### Expected skill behavior

- Detects high-frequency state updates and remount churn.
- Replaces frame-critical state updates with ref mutation in `useFrame`.
- Suggests `frameloop=\"demand\"` plus `invalidate()` where suitable.
- Flags anti-patterns like `setState` inside `useFrame`.

## Demo 3: Asset and loading optimization

### Prompt

"Our GLB and textures are too heavy for mobile. Optimize loading pipeline with quality controls."

### Expected skill behavior

- Suggests glTF inspection and compression pipeline.
- Recommends Draco/Meshopt evaluation and KTX2 strategy.
- Verifies decoder/transcoder setup correctness.
- Adds loading prioritization and progressive quality guidance.

## Live demonstration ideas

To increase adoption, publish one of these and link it in README:

- 90-second screen recording showing one optimization pass.
- GitHub issue-to-fix walkthrough as a short video.
- Prompt-to-result terminal recording with before/after metrics.
