# Code Reviews

Reviewing of PRs

### 🥅 Goals

* Improve code quality
* Grow by learning
* Develop shared understanding

## Pull Request

Changes should go through Pull Request (PR) for code review.

#### Templates

```markdown
## Description

Add description

## References

- [JIRA card](https://identifi.atlassian.net/browse/JAM-1)

## Platform

- [ ] Backend
- [ ] Web
- [ ] Mobile
- [ ] DevOps
- [ ] QA Automation

## Types of changes

- [ ] Bug fix
- [ ] Non-breaking change
- [ ] Breaking change

## Affected Components

- [ ] Admin
- [ ] API
- [ ] Integration
- [ ] CI/CD
- [ ] Terraform
- [ ] Packer
- [ ] Others
```



## Typescript Checklist

* [ ] Does the code follow the code standards?
* [ ] Are tests arranged correctly with the Arrange/Act/Assert pattern and properly documented in this way?
* [ ] Are unit tests used where possible?

### ESLint

```json
{
  "parser": "@typescript-eslint/parser",
  "plugins": ["@typescript-eslint", "import"],
  "extends": [
    "airbnb-base",
    "plugin:@typescript-eslint/recommended",
    "plugin:import/typescript"
  ],
  "settings": {
    "import/resolver": {
      "typescript": {}
    }
  },
  "env": {
    "node": true,
    "mocha": true
  },
  "rules": {
    "max-len": ["error", 128],
    "import/extensions": "off",
    "func-names": "off",
    "semi": "off",
    "no-shadow": "off",
    "@typescript-eslint/no-shadow": ["error"],
    "import/no-extraneous-dependencies": "off",
    "@typescript-eslint/semi": ["error"],
    "@typescript-eslint/explicit-module-boundary-types": "off",
    "import/prefer-default-export": "off",
    "@typescript-eslint/ban-types": "off",
    "class-methods-use-this": "off",
    "object-curly-spacing": "off",
    "@typescript-eslint/object-curly-spacing": ["error", "always"],
  }

}
```

### Setting up Prettier

```json
{
  "singleQuote": true,
  "trailingComma": "all",
  "tabWidth": 2,
  "semi": true
}
```

### Pre-commit hooks

We're using [`husky`](https://github.com/typicode/husky)

```
#!/bin/sh
. "$(dirname "$0")/_/husky.sh"

# your command here
```

### Auto formatting with VS Code

```json
{
  "editor.codeActionsOnSave": {
    "source.fixAll.eslint": true
  },
}
```

## Slack Bot Integration

There are bots to help signal for code reviews.

Please see, [HOV DevOps Bot](https://github.com/HighOutputVentures/hov-devops-bot)

## Recipes

### Gherkin

#### Each `Scenario` should be independent

It could run alone and should not rely upon other scenarios to run correctly.

### Resources

1. [High Output Engineering -- Code Review](https://www.notion.so/highoutput/Code-Review-80d4445e3527418a96e922bab557bd4b)
