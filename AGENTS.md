# Repository Guidelines

## Project Structure & Module Organization
This repo packages Gemini CLI extension skills.
- `skills/<skill-name>/SKILL.md`: core instruction set for each specialist.
- `README.md`: install/activation workflow.
- `gemini-extension.json`: extension metadata and registration.
- `GEMINI.md`: project-specific collaboration conventions.

Keep each skill independently usable and aligned with the activation patterns documented in `README.md`.

## Build, Test, and Development Commands
There is no traditional build; validate extension metadata and skill content.

```bash
# Link extension locally
gemini extensions link .

# List skill definitions
find skills -mindepth 2 -maxdepth 2 -name SKILL.md | sort

# Check required frontmatter keys
rg -n "^(name|description):" skills/*/SKILL.md

# Validate JSON metadata
python3 -m json.tool gemini-extension.json >/dev/null
```

## Coding Style & Naming Conventions
- Use YAML frontmatter in every `SKILL.md`.
- Required fields: `name`, `description`.
- Keep names lowercase kebab-case and in sync with folder names.
- Write short, direct instructions with concrete activation examples (`activate <skill>`).
- Avoid duplicate scope across skills; each one should own a clear responsibility.

## Testing Guidelines
- Frontmatter validation is required for every modified skill.
- After changes, re-link the extension and run one real activation prompt per edited skill.
- If metadata changes, verify `gemini-extension.json` remains valid JSON.

## Commit & Pull Request Guidelines
Recent commits follow semantic style (`feat:`, `rename`, cleanup-focused updates).
- Prefer Conventional Commits (`feat:`, `fix:`, `docs:`, `chore:`).
- Keep one logical concern per commit.
- PRs should include changed skills, activation examples, and manual verification notes.

## Security & Configuration Tips
- Do not commit local credentials, tokens, or machine-specific config.
- Keep generated cache/artifact files out of this repository.
