pre-commit-checkstyle
===

pre-commit hooks for checkstyle

Requirements
---

- `pre-commit`
- git project
  - with `gradle` checkstyle plugin
  - with `maven` checkstyle plugin

Install
---

1. Create `.pre-commit-config.yaml` to your project.

```yaml
repos:
- repo: https://github.com/junghoon-vans/pre-commit-checkstyle
    rev: v1.2.0
    hooks:
    - id: gradle-checkstyle
    - id: gradle-checkstyle-main
    - id: gradle-checkstyle-test
    - id: maven-checkstyle
    - id: maven-checkstyle-report
```

2. Run `pre-commit install` command.

Hooks
---

### `gradle-checkstyle`

- Runs Checkstyle against `all Java source` files.

### `gradle-checkstyle-main`

- Runs Checkstyle against the `production Java source` files.
- Generates an `HTML report` on any violations.

### `gradle-checkstyle-test`

- Runs Checkstyle against the `test Java source` files.
- Generates an `HTML report` on any violations.

### `maven-checkstyle`

- Runs Checkstyle against `all Java source` files.

### `maven-checkstyle-report`

- Generates an `HTML report` on any violations.
