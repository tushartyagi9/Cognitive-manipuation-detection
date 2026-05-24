# CogniGuard — Cognitive Manipulation Detection

CogniGuard is a research and prototype toolkit for detecting cognitive manipulation in text (especially email). It provides a three-tier pipeline:

- Tier 1: fast binary gating (legitimate vs manipulative)
- Tier 2: seven-class semantic typing (e.g., Fear Induction, Urgency Manipulation)
- Tier 3: rule-based escalation for low-confidence or high-risk cases

This repository contains the frontend (Vite + React), an Express backend, Python scripts for dataset preparation and inference tooling, and evaluation assets.

Getting started (development)

1. Install dependencies (root, client or server as needed):

```bash
# install frontend dependencies
cd Mindguard
npm install

# from repo root you can also install server deps if used
cd Mindguard
npm run dev
```

2. Run the frontend (Vite):

```bash
cd Mindguard
npm run dev
```

3. Start the backend (Express):

```bash
cd Mindguard
npm run dev:server
```

Notes
- Environment variables: copy `Mindguard/.env.example` to `Mindguard/.env` and fill in keys.
- Package name updated to `cogniguard` in client metadata. The source folder remains `Mindguard` to preserve history.
- Dataset utilities and scripts live under `Mindguard/scripts` and `Mindguard/server/data`.

Contributing
- Open an issue or submit a PR. For dataset changes, follow the benchmark workflow in `Mindguard/docs/BENCHMARK_WORKFLOW.md`.

License
- (Add your preferred license here)

