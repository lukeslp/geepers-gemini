# geepers-gemini

Generated Gemini extension mirror for geepers skills.

## Source of Truth

This repository is synced from canonical skills in:
- `https://github.com/lukeslp/geepers`
- Canonical path: `skills/source/`

Direct edits to `skills/` in this repo are blocked by CI. Make changes in canonical source, then sync.

## What Is Here

- `skills/`: generated skill folders for Gemini workflows
- `gemini-extension.json`: generated extension metadata
- `aliases.generated.json`: migration aliases
- `.github/workflows/mirror-readonly-guard.yml`: mirror protection

## Install

```bash
gemini extensions link .
```

## Sync Workflow

From canonical repo (`/home/coolhand/geepers`):

```bash
python3 scripts/validate-skills.py --strict
python3 scripts/build-platform-packages.py --platform gemini --clean
bash scripts/sync-mirrors.sh --platform gemini --delete --skip-build
bash scripts/report-drift.sh --platform gemini --skip-missing
```

## License

MIT
