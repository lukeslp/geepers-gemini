# Geepers Gemini

`geepers-gemini` is a native Gemini CLI extension designed for high-stakes engineering. It transforms your CLI into a coordinated team of specialists, each governed by expert-level instruction sets.

## Why Geepers?

In complex codebases, general-purpose prompts often miss the nuances of architecture and safety. Geepers provides:

- **Surgical Precision**: Tools like `geepers-scalpel` ensure that edits to massive files are localized and non-destructive.
- **Model Intelligence**: Automated tiering that leverages the latest 2026 flagship models (Opus 4.6, GPT-5) for strategy, while using efficient models for routine tasks.
- **Parallel Workflows**: Built-in mandates to execute independent discovery and editing tasks concurrently.

## The Specialist Team

| Expert | Activation | Focus |
|---|---|---|
| **The Surgeon** | `activate geepers-scalpel` | High-precision edits to complex files. |
| **The Architect**| `activate geepers-critic` | Deep architectural review and tech-debt identification. |
| **The Scout**    | `activate geepers-scout` | Rapid system mapping and external API research. |
| **The Auditor**  | `activate geepers-security` | Vulnerability scanning and secret detection. |
| **The QA Lead**  | `activate geepers-test` | Automated test suite generation and verification. |
| **The Editor**  | `activate geepers-humanizer` | Refining AI output for professional human clarity. |

## Quick Start

1. **Link the extension**:
   ```bash
   cd packages/geepers-gemini && gemini extensions link .
   ```
2. **Engage a specialist**:
   ```bash
   activate geepers-scout
   "Map out the dependencies in the DashCam prediction worker."
   ```

## Development

Geepers follows a strict **"Safety First, Fact-Based"** philosophy. All contributions must adhere to the conventions defined in `GEMINI.md`.
