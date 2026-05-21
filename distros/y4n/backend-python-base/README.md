---
name: y4n/backend-python-base
display_name: Backend Python Base
description: Debian Slim environment for Python API development and testing
status: stable
devcontainer: debian-slim
tags: [python, api, fastapi, postgres, debian]
packages: [cli-essentials, git-extras, zsh-config, neovim-config, python-runtime, api-dev, db-clients, ruff]
---

# Backend Python Base

Debian Slim devpod for Python API development. Primary use: running tests and dev servers inside the container. IDE and coding happen locally.

## Contents

| Layer | Packages |
|-------|---------|
| Shared | cli-essentials, git-extras, zsh-config, neovim-config |
| Role | python-runtime, api-dev, db-clients, ruff |

## Usage

```yaml
# dpod.yaml
distro: y4n/backend-python-base@v0.1.0
```

## Common overrides

Add power-user TUI tools:

```yaml
distro: y4n/backend-python-base@v0.1.0
packages:
  - tui-power@v0.1.0
```
