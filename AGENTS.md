# Repository Guidelines

## Project Structure & Module Organization

This repository currently contains product documentation rather than executable code:

- `README.md` — short project overview.
- `PRD.md` — authoritative product requirements and curriculum design decisions.
- Planned skill layout (per `PRD.md`): `SKILL.md`, `references/`, `templates/`, `rubrics/`, and `examples/`.

Keep research and reusable guidance in `references/`, output skeletons in `templates/`, review criteria in `rubrics/`, and complete examples in `examples/`. Update `PRD.md` when a structural or product decision changes.

## Build, Test, and Development Commands

No build, dependency, or test commands are configured yet. For documentation-only changes, inspect the diff with:

```powershell
git diff --check
git diff -- README.md PRD.md AGENTS.md
```

When implementation begins, add the canonical setup, lint, and test commands here and keep them runnable from the repository root.

## Coding Style & Naming Conventions

Use Markdown with one top-level heading per document, ATX headings, short paragraphs, and fenced code blocks for examples. Prefer clear English filenames in kebab-case (for example, `curriculum-design.md`); preserve the existing uppercase names for top-level contract files such as `PRD.md` and `SKILL.md`. Keep curriculum language tool-agnostic and explain concepts before vendor-specific examples.

## Testing Guidelines

There is no automated test suite or coverage requirement yet. Validate documentation changes with `git diff --check`, verify links and code examples manually, and ensure terminology remains consistent with `PRD.md`. Future skill behavior should add focused examples or tests for curriculum generation, tool-selection, research gates, and coherence review.

## Commit & Pull Request Guidelines

Only an initial `first commit` exists, so no established convention is present. Use concise imperative subjects (for example, `Add curriculum output template`) and keep each commit focused. Pull requests should explain the user-facing or documentation impact, link the relevant issue or PRD section, and include representative output or screenshots when changing generated formats or examples.

## Security & Configuration Tips

Do not commit API keys, private research data, or tool credentials. Keep technology claims and freshness assessments traceable to sources, and flag content that may become outdated.



## Git Automation & Deployment

When a task or feature implementation is successfully completed and passes all validation checks, execute the following auto-commit and push sequence:

1. **Stage Changes:** Stage all modified and tracked files.

   ```bash
   git add .
   ```
2. **Generate Commit Message:** Write a structured commit message following Conventional Commits format (e.g., `feat: add automated push instructions`).
3. **Commit Code:** Run the local commit.

   ```bash
   git commit -m "<type>(<scope>): <short summary>"
   ```
4. **Push to Remote:** Push changes to the current active branch automatically.

   ```bash
   git push origin HEAD
   ```

### Automation Constraints

- **Strict Verification:** Never auto-push if tests fail, if linting errors are present, or if compile errors exist.
- **Credential Safety:** Ensure no personal secrets (`.env`, private keys) are staged. Check `.gitignore` alignment before pushing.
- **Conflict Handling:** If a push fails due to upstream changes, pull with rebase (`git pull --rebase origin main`), resolve conflicts, and re-run validation before attempting another push.
