# Precommit hooks

An example `.pre-commit-config.yaml` I like to use:

```yaml
fail_fast: true
repos:
  - repo: http://github.com/pre-commit/pre-commit-hooks
    rev: v3.4.0
    hooks:
      - id: no-commit-to-branch
        args: ['--pattern', '^(?!((bugfix|feature)\/.*)$).*']  # see https://www.devwithimagination.com/2020/04/13/git-commit-hooks-for-branch-naming-pre-commit/
  - repo: http://github.com/pre-commit/pre-commit-hooks
    rev: v3.4.0
    hooks:
      - id: check-added-large-files
  - repo: http://github.com/pre-commit/pre-commit-hooks
    rev: v3.4.0
    hooks:
      - id: check-merge-conflict
  - repo: https://github.com/pre-commit/pygrep-hooks
    rev: v1.9.0
    hooks:
      - id: python-no-eval
  - repo: https://github.com/charliermarsh/ruff-pre-commit
    rev: 'v0.0.255'
    hooks:
      - id: ruff
        args: [--fix, --show-fixes]
  - repo: http://github.com/psf/black
    rev: 22.10.0
    hooks:
      - id: black
        language_version: python
        exclude: .pyi$
        args: [--line-length=160]
  - repo: https://github.com/Lucas-C/pre-commit-hooks-safety
    rev: v1.3.0
    hooks:
      - id: python-safety-dependencies-check
        files: ^requirements.txt$
```
