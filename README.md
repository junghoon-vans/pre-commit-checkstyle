pre-commit-checkstyle
===

pre-commit hooks for checkstyle

Requirements
---

- `pre-commit`
- `gradle project` installed checkstyle

Install
---

1. Create `.pre-commit-config.yaml` to your project.

```yaml
repos:
- repo: https://github.com/junghoon-vans/pre-commit-checkstyle
    rev: v1.0.0
    hooks:
    - id: gradle-checkstyle-main
    - id: gradle-checkstyle-test
```

2. Run `pre-commit install` command.

Hooks
---

### `gradle-checkstyle-main`

Run `checkstyleMain` using gradle

### `gradle-checkstyle-test`

Run `checkstyleTest` using gradle
