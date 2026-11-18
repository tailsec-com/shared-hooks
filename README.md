# Shared Git Hooks

Husky-based git hooks shared across Tailsec repos.

## Usage

Install hooks when setting up a new repo:

```bash
npm install --save-dev husky
npx husky install
```

Or use the shared hooks:

```bash
git config core.hooksPath shared-hooks/.husky
```

## Hooks

- **pre-commit**: Runs typecheck and tests
- **pre-push**: Runs full typecheck and lint

## Adding to a new repo

1. Copy `.husky/` directory to the repo
2. Run `npm install && npx husky install`
3. Or symlink to `shared-hooks/.husky`

[![advertisement](https://ads.servead.net/i/2c847c68-27cf-45bc-9687-84962dfebd21.svg)](https://ads.servead.net/c/2c847c68-27cf-45bc-9687-84962dfebd21)
