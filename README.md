# gitleaks

## Installation Guide

1. Install `gitleaks`

```sh
brew install gitleaks
```

2. Install `pre-commit`, this tool is used for create pre-commit hook

```sh
brew install pre-commit
```

3. Ensure that there is file `.pre-commit-config.yaml` with this following content (you can copy content from this repository)

```yaml
repos:
  - repo: https://github.com/zricethezav/gitleaks
    rev: v8.15.0
    hooks:
      - id: gitleaks
```

4. (Optional) In case want to use default config

```sh
pre-commit autoupdate
```

5. you can use your own config by copy `.gitleaks.toml` from this repository to your repository (root folder)

6. Create hook by running this command in root folder of your repository

```sh
pre-commit install
```

You're all set!.
