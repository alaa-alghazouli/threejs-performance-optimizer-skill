# Use Cases

## 1) Game scene drops FPS during combat

- Symptoms: frame spikes, unstable camera movement.
- Skill focus: draw-call reduction, shadow scope tuning, postprocessing budget.

## 2) Product configurator drains laptop battery

- Symptoms: continuous rendering despite static scene.
- Skill focus: on-demand rendering, event-driven invalidation, adaptive DPR.

## 3) Massive repeated environment props

- Symptoms: thousands of similar meshes with poor FPS.
- Skill focus: `InstancedMesh`, material reuse, static merge strategy.

## 4) Slow startup on mobile networks

- Symptoms: delayed first interactive render.
- Skill focus: GLB/texture compression, staged loading, decoder/transcoder setup.

## 5) Memory leaks after route changes

- Symptoms: increasing memory usage and eventual instability.
- Skill focus: explicit disposal flow for geometries, materials, textures, targets, skeletons.

## 6) R3F pointer interactions are laggy

- Symptoms: stutter while dragging, hover, or camera controls.
- Skill focus: frame-loop mutation via refs, avoid `setState` in high-frequency paths.

## 7) Visual quality regresses after optimization

- Symptoms: blurry textures or lighting artifacts.
- Skill focus: measurable quality-performance tradeoffs and rollback criteria.

## 8) Mixed WebGPU/WebGL compatibility concerns

- Symptoms: uncertain behavior across devices.
- Skill focus: renderer initialization strategy, fallback planning, feature-safe recommendations.
