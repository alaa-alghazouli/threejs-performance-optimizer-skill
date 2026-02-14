# threejs-performance-optimizer

[![CI](https://github.com/alaa-alghazouli/threejs-performance-optimizer-skill/actions/workflows/ci.yml/badge.svg)](https://github.com/alaa-alghazouli/threejs-performance-optimizer-skill/actions/workflows/ci.yml)
[![Latest Release](https://img.shields.io/github/v/release/alaa-alghazouli/threejs-performance-optimizer-skill)](https://github.com/alaa-alghazouli/threejs-performance-optimizer-skill/releases)
[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](./LICENSE)

Public AI skill that helps coding agents optimize Three.js and React Three Fiber performance using a profile-first, docs-aligned workflow.

## Why this skill

Most Three.js performance advice online is either generic or outdated. This skill turns optimization into a repeatable process:

- Diagnose bottlenecks before touching code (CPU, GPU, memory, loading).
- Prioritize highest-impact fixes in ROI order.
- Apply current guidance from official Three.js and R3F docs.
- Produce measurable before/after results with tradeoffs and verification.

## Quick start

1. Download the packaged skill: `dist/threejs-performance-optimizer.skill` or from the [latest release](https://github.com/alaa-alghazouli/threejs-performance-optimizer-skill/releases/latest).
2. Import it into your AI CLI/tool that supports `.skill` bundles.
3. Trigger it with prompts like:
   - "Optimize my Three.js scene, FPS is unstable"
   - "Reduce draw calls in this R3F app"
   - "Fix memory leaks in this Three.js route transition"

## Demo and examples

- Interactive prompt walkthrough: [`docs/DEMO.md`](docs/DEMO.md)
- Real-world use cases: [`docs/USE_CASES.md`](docs/USE_CASES.md)
- Skill behavior contract and reference: [`docs/API_REFERENCE.md`](docs/API_REFERENCE.md)

## What the skill covers

- Renderer and frame-loop strategy (continuous vs on-demand rendering)
- Draw-call reduction (instancing, batching, static merge tradeoffs)
- Asset pipeline optimization (glTF, Draco/Meshopt, KTX2)
- Lighting, shadows, postprocessing cost control
- Memory lifecycle and explicit disposal correctness
- R3F-specific anti-pattern prevention (`setState` in frame loops, remount churn)
- Outdated-guidance guardrails to avoid stale APIs

## Repository structure

- `threejs-performance-optimizer/SKILL.md` - main instructions and optimization workflow.
- `threejs-performance-optimizer/references/*` - focused, load-on-demand reference docs.
- `dist/threejs-performance-optimizer.skill` - distributable packaged skill.
- `docs/*` - demos, use cases, API reference, launch playbook, and showcase.

## Contributing

Contributions are welcome. Start with:

- [`CONTRIBUTING.md`](CONTRIBUTING.md)
- `good first issue` and `help wanted` labels in the issue tracker

## Community

- Discussions: use GitHub Discussions for questions and ideas.
- Showcase your results: add your project to [`docs/SHOWCASE.md`](docs/SHOWCASE.md).

## Contributors

Thanks to everyone improving this skill. Add yourself in a PR after your first merged contribution.
