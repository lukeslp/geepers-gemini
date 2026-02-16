# Foresight

`foresight` is a native Gemini CLI extension and multi-agent orchestration suite. It transforms the Gemini CLI into a team of specialized expert "personas" capable of handling everything from high-precision code surgery to deep architectural research.

## Features

- **Expert Skills**: Specialized instruction sets (`SKILL.md`) for different domains.
- **Strategic Tiering**: Optimized for early 2026 state-of-the-art models (Opus 4.6, GPT-5, Sonnet 4.5).
- **Task-Specific Workflows**: Dedicated workflows for planning, building, debugging, and auditing.

## Installation

```bash
gemini extensions install lukeslp/foresight
```

## Available Skills

| Skill | Activation Command | Purpose |
|---|---|---|
| **Scalpel** | `activate geepers-scalpel` | Surgical, high-precision code edits. |
| **Critic** | `activate geepers-critic` | Objective code review and optimization. |
| **Scout** | `activate geepers-scout` | Deep research and system mapping. |
| **Planner** | `activate geepers-planner` | Task prioritization and session strategy. |
| **Builder** | `activate geepers-builder` | Feature implementation and scaffolding. |
| **Diag** | `activate geepers-diag` | Debugging and root cause analysis. |
| **Security** | `activate geepers-security` | Vulnerability auditing and data protection. |
| **Test** | `activate geepers-test` | Comprehensive test suite generation. |
| **Team** | `activate geepers-team` | Lead orchestration and cross-agent coordination. |

## Usage

Once the extension is installed, you can activate any skill to put the agent into a specialized mode:

```bash
# Example: Using the Scalpel for a complex edit
activate geepers-scalpel
"Modify the payment logic in large_file.py to support the new API."
```

## Contributing

See `GEMINI.md` for development conventions and `QUICK_REFERENCE.md` for a task-to-agent mapping.
