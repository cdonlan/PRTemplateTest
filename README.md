# PRTemplateTest

## Using Pull Request Templates

This repository has multiple PR templates to help you create well-structured pull requests. Each template is designed for a specific type of change.

### Available Templates

- **Bug Fix** (`bug_fix.md`) - For fixing bugs
- **Feature** (`feature.md`) - For adding new features
- **Documentation** (`documentation.md`) - For documentation updates
- **Refactor** (`refactor.md`) - For code refactoring

### How to Select a Template

When creating a pull request, you can select a specific template by adding a query parameter to the PR creation URL:

#### Method 1: Using URL Query Parameters

Add `?template=TEMPLATE_NAME.md` to the compare URL:

```
https://github.com/cdonlan/PRTemplateTest/compare/main...YOUR_BRANCH?template=bug_fix.md
https://github.com/cdonlan/PRTemplateTest/compare/main...YOUR_BRANCH?template=feature.md
https://github.com/cdonlan/PRTemplateTest/compare/main...YOUR_BRANCH?template=documentation.md
https://github.com/cdonlan/PRTemplateTest/compare/main...YOUR_BRANCH?template=refactor.md
```

Replace `YOUR_BRANCH` with your actual branch name.

#### Method 2: Quick Links

Use these direct links when creating a PR from your branch:

- [Create Bug Fix PR](../../compare/main?template=bug_fix.md)
- [Create Feature PR](../../compare/main?template=feature.md)
- [Create Documentation PR](../../compare/main?template=documentation.md)
- [Create Refactor PR](../../compare/main?template=refactor.md)

#### Method 3: Manual Selection

1. Start creating a pull request normally
2. In the PR description, manually copy the content from the desired template in `.github/PULL_REQUEST_TEMPLATE/`

### Template Location

All templates are stored in: `.github/PULL_REQUEST_TEMPLATE/`
