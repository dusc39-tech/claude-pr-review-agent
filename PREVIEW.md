# Claude PR Review Agent — vista previa

Esta muestra enseña el formato de salida. La edición completa incluye el CLI, instalación, pruebas automatizadas y dos ejemplos revisados.

## Summary

The pull request adds a read-only review command that fetches a public GitHub diff and produces a consistent Markdown report. It does not check out, execute, or modify the reviewed repository.

## Risks

- Medium — the review depends on the public diff being available and complete.
- Low — a model-generated review should be verified by a human before merging.

## Improvement Suggestions

- Keep the default workflow read-only.
- Use --post-comment only with an explicit GitHub token.
- Add repository-specific tests for unusual diff formats.

## Confidence Score

Medium — the structure is validated, but human review remains necessary for security-sensitive or high-impact changes.

## Requirements

- Python 3.9+
- Authenticated Claude Code CLI
- GitHub CLI is optional

The downloadable product is available in Individual and Team variants.
