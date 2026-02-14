# Skill Reference

## Skill identity

- Name: `threejs-performance-optimizer`
- Package: `dist/threejs-performance-optimizer.skill`

## Trigger intent

Use for requests about:

- low FPS, frame drops, stutter/jank
- high draw calls or expensive rendering paths
- Three.js or R3F memory leaks/disposal problems
- mobile 3D performance bottlenecks
- GLB/texture loading and compression optimization
- on-demand rendering and invalidate patterns

## Optimization contract

Every optimization output should include:

1. Bottleneck diagnosis
2. Ordered action plan
3. Risk and compatibility notes
4. Verification criteria and expected metric movement

## Reference modules

- `references/performance-workflow.md`
- `references/renderer-and-loop-patterns.md`
- `references/assets-and-loaders.md`
- `references/draw-calls-materials-lighting.md`
- `references/memory-and-disposal.md`
- `references/r3f-rules.md`
- `references/outdated-guidance.md`

## Guardrails

- Prefer current official docs over old snippets.
- Avoid deprecated renderer/API recommendations.
- Treat hard thresholds as context-dependent heuristics.
- Avoid blanket statements without measurement.
