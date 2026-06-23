# Attention Optimisation

Please apply the following optimisation wherever possible to protect your precious context window:

- [Code Interface Reading](#code-interface-reading)
- [Avoid STDOUT Explosion](#avoid-stdout-explosion)

## Code Interface Reading

When exploring a python, javascript/typescript or C# codebase at a high level (not diving deeply into a specific part of the codebase), use the `script_summary` CLI tool for viewing file contents.

Examples:

```bash
cd frontend/src/pages/JobHistory && script_summary index.tsx
cd backend/apps/jobs && script_summary service.py
```

This CLI tool shows you only the interfaces, omitting the implementation detail.

## Avoid STDOUT Explosion

When running terminal commands which often have very large output (such as `cat`, `docker`, `find`, `grep`, `rg`, `fd`, `git`, `jq`, `kubectl`, `ls -R`, `tree`, `du`, `locate`, `stat`, `ps`, `top`, `lsof`, `systemctl` etc.), first pipe your command output into `| wc -l` to check it's length. If it's more than 500 lines, you should refine your command (view head/tail first, apply filtering, limit scope, produce summary views first, grep within result etc.).

When using `fd` (or `find`) for listing files, you can often reduce the output size significantly by excluding common package and caching directories like this:

```bash
fd . --type f \
--exclude .git \
--exclude .venv \
--exclude venv \
--exclude __pycache__ \
--exclude coverage \
--exclude .pytest_cache \
--exclude .mypy_cache \
--exclude .ruff_cache \
--exclude node_modules
```
