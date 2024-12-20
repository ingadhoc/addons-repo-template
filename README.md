[![ci](https://github.com/ingadhoc/addons-repo-template/actions/workflows/ci.yml/badge.svg)](https://github.com/ingadhoc/addons-repo-template/actions/workflows/ci.yml)

# Adhoc Addons Repository Template

Template to bootstrap an addons repository.

## Why?

We have dozens of repos. Most of them look the same, and most of them need specific-but-similar configurations for CI,
code quality, dependency management, etc.

## How to use?

This is a template based on [Copier](https://github.com/pykong/copier), go there to read its docs to know how it works.

## Requirements

Using pipx (recommended):

```bash
# Install copier and pre-commit if missing
pipx install copier
pipx install pre-commit
pipx ensurepath
```

## Quick start

### Initialize a new repository

```bash
# Clone this template and answer its questions
copier copy --trust https://github.com/ingadhoc/addons-repo-template.git awesome-addons
# Commit that
cd awesome-addons
git add .
git commit -am 'Initialize ✨'
```

### Convert an existing repo to use this template

```bash
# Clone the repo locally
git clone https://github.com/ingadhoc/awesome-addons.git
cd awesome-addons
# Apply the template and answer its questions
copier copy --trust https://github.com/ingadhoc/addons-repo-template.git .
# Commit that
git add .
git commit -am 'Initialize ✨'
```

### Update a repo to pull latests changes from this template

```bash
copier update --trust
```
