[![Minimal node version](https://img.shields.io/static/v1?label=node&message=%3E=14.16&logo=node.js&color)](https://nodejs.org/about/releases/)
[![Minimal npm version](https://img.shields.io/static/v1?label=npm&message=%3E=6.14.12&logo=npm&color)](https://github.com/npm/cli/releases)
[![Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https://GitHub.com/stephen-shopopop/eslint-config/graphs/commit-activity)
[![Linux](https://svgshare.com/i/Zhy.svg)](https://svgshare.com/i/Zhy.svg)
[![macOS](https://svgshare.com/i/ZjP.svg)](https://svgshare.com/i/ZjP.svg)
[![Visual Studio Code](https://img.shields.io/badge/--007ACC?logo=visual%20studio%20code&logoColor=ffffff)](https://code.visualstudio.com/)

# Eslint configuration

## Description

Eslint configuration for typescript

## Usage

### Install

Add .npmrc file in your project

> @stephen-shopopop:registry=https://npm.pkg.github.com

```bash
npm add -D eslint @stephen-shopopop/eslint-config
```

### Config `.eslintrc`

```json
{
  "extends": "@stephen-shopopop/eslint-config"
}
```

> You don't need `.eslintignore` normally as it has been provided by the preset.

### Add script for package.json

For example:

```json
{
  "scripts": {
    "lint": "eslint .",
    "lint:fix": "npm run lint -- --fix",
  }
}
```

For example typescript:

```json
{
  "scripts": {
    "lint": "eslint . --ext .ts",
    "lint:fix": "npm run lint -- --fix",
  }
}
```

### Config VS Code auto fix

Create `.vscode/settings.json`

```json
{
  "prettier.enable": false,
  "editor.codeActionsOnSave": {
    "source.fixAll.eslint": true
  }
}
```

## DETAILS

**ESLINT:**

- [Typescript ESLint](https://typescript-eslint.io)
- [ESLint configuration](https://eslint.org/docs/user-guide/configuring/)
- [ESLint rules](https://eslint.org/docs/rules/)
- [ESLint standard](https://www.npmjs.com/package/eslint-config-standard)
- [ESLint unicorn](https://github.com/sindresorhus/eslint-plugin-unicorn)
- [ESLint comments](https://mysticatea.github.io/eslint-plugin-eslint-comments/)
- [ESLint import](https://github.com/import-js/eslint-plugin-import)
- [ESLint json](https://www.npmjs.com/package/eslint-plugin-jsonc)
- [ESLint promise](https://www.npmjs.com/package/eslint-plugin-promise)
- [ESLint yaml](https://www.npmjs.com/package/eslint-plugin-yml) (for CI)
- [ESLint prettier](https://github.com/prettier/eslint-config-prettier)
- [ESLint node](https://www.npmjs.com/package/eslint-plugin-n)
- [ESLint parser json](https://www.npmjs.com/package/jsonc-eslint-parser)
- [ESLint parser yaml](https://www.npmjs.com/package/yaml-eslint-parser)


## Contributing

1. npm run lint - eslint test config
2. npm run release - Release library && publish

## Docs

### Summary

- [library & tools](tools.md)

### Package maintenance

A modern cli tool that keeps your deps fresh

```bash
npx taze
```
