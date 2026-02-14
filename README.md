# threejs-performance-optimizer

Public AI skill for optimizing Three.js and React Three Fiber projects with a profile-first workflow.

## What this skill does

- Diagnoses bottlenecks (CPU, GPU, memory, loading) before changing code.
- Prioritizes the highest-ROI fixes first: assets, draw calls, render loop policy, lighting/post, cleanup.
- Applies current Three.js and R3F guidance, with explicit stale-advice guardrails.
- Produces measurable before/after recommendations with tradeoffs and verification steps.

## Typical trigger prompts

- "Optimize my Three.js scene, FPS is unstable"
- "Reduce draw calls in this R3F app"
- "Fix stutter when orbiting camera"
- "Improve mobile performance for this WebGL/WebGPU scene"
- "Audit my memory leaks in Three.js"
- "Set up Draco/KTX2 for my GLB pipeline"
- "Switch this scene to demand rendering"
- "Tune lights, shadows, and postprocessing cost"

## Example usage prompts

- "My scene drops to 28 FPS on mobile. Diagnose and optimize with the least visual loss."
- "I have 2,000 repeated meshes in Three.js. Refactor for fewer draw calls and verify impact."
- "In R3F, pointer interactions feel janky. Optimize frame-loop and state patterns."
- "Set up GLTFLoader with Draco + KTX2 correctly and list common pitfalls."
- "I suspect memory leaks after route changes. Add a proper disposal checklist and fixes."

## Repository contents

- `threejs-performance-optimizer/SKILL.md`: main skill instructions and workflow.
- `threejs-performance-optimizer/references/*`: focused references for renderer setup, assets, draw calls, memory/disposal, and R3F.
- `dist/threejs-performance-optimizer.skill`: packaged distributable skill file.

## Source policy

This skill is designed to be docs-aligned and version-safe:

- Prefer official docs over blog heuristics.
- Treat hard thresholds as heuristics, not universal rules.
- Avoid deprecated or outdated API guidance.
