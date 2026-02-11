# Pull Request Template Guide

## Overview

This repository uses multiple pull request templates to help contributors create well-structured PRs based on the type of change being made.

## Available Templates

### 1. Bug Fix Template
**File:** `bug_fix.md`  
**Use for:** Fixing bugs, issues, or errors in the codebase

**Key sections:**
- Description of the bug
- Root cause analysis
- Solution approach
- Testing performed

### 2. Feature Template
**File:** `feature.md`  
**Use for:** Adding new features or functionality

**Key sections:**
- Feature description
- Motivation and use case
- Implementation details
- Testing and documentation

### 3. Documentation Template
**File:** `documentation.md`  
**Use for:** Updating or adding documentation

**Key sections:**
- Documentation changes
- Motivation for the update
- Review checklist

### 4. Refactor Template
**File:** `refactor.md`  
**Use for:** Code refactoring without changing functionality

**Key sections:**
- Refactoring description
- Motivation
- Impact assessment
- Testing to ensure no regression

## How to Use Templates

### Option 1: URL Query Parameters (Recommended)

When you're ready to create a pull request, modify the GitHub compare URL to include the template parameter:

```
https://github.com/OWNER/REPO/compare/BASE_BRANCH...YOUR_BRANCH?template=TEMPLATE_NAME.md
```

**Example for this repository:**
```
https://github.com/cdonlan/PRTemplateTest/compare/main...my-bug-fix?template=bug_fix.md
```

### Option 2: Direct Links from README

The README.md file contains quick links for each template type. Click the appropriate link for your change type.

### Option 3: Manual Copy-Paste

1. Navigate to `.github/PULL_REQUEST_TEMPLATE/` in the repository
2. Open the desired template file
3. Copy the template content
4. Create your PR and paste the template into the description

## Best Practices

1. **Choose the right template** - Select the template that best matches your change type
2. **Fill in all sections** - Complete all relevant sections in the template
3. **Remove unused sections** - If a section doesn't apply, you can remove it with a note
4. **Keep it concise** - Be clear and concise in your descriptions
5. **Link related issues** - Always link to related issues or discussions

## Creating New Templates

To add a new template type:

1. Create a new `.md` file in `.github/PULL_REQUEST_TEMPLATE/`
2. Use a descriptive filename (e.g., `hotfix.md`, `security_fix.md`)
3. Structure the template with clear sections using markdown
4. Update the README.md to document the new template

## GitHub Behavior Notes

- If you have only ONE template file named `pull_request_template.md` in `.github/`, GitHub automatically uses it for all PRs
- If you have MULTIPLE templates in `.github/PULL_REQUEST_TEMPLATE/`, users must explicitly select which one to use via the query parameter
- Without specifying a template parameter, GitHub will show a blank PR description when multiple templates exist
