---
name: vllm-skills-contributing
description: Guidelines for contributing new or updated skills to this repository, including required structure and documentation updates.
---

# Contributing to vllm-skills

Use this skill when you want to add, update, or review skills in this repository.

## Contribution workflow

1. Create or update a skill directory under `skills/`.
2. Ensure each skill has a `SKILL.md` file with YAML frontmatter:
   ```yaml
   ---
   name: your-skill
   description: Brief description of what this skill does
   ---
   ```
3. Add optional supporting files as needed:
   - `scripts/`
   - `references/`
   - `assets/`
4. Update `README.md`:
   - Add or update the skill in the Skills Index.
   - Document usage examples if needed.
5. If adding/removing skills, update `.claude-plugin/marketplace.json` so marketplace installs stay accurate.
6. Validate changed scripts (for example, use `bash -n` for shell scripts) before opening a PR.

## Notes

- Keep changes focused and minimal.
- Do not commit secrets, tokens, or credentials.
- Follow existing formatting and naming conventions in this repository.
