[![Minimal node version](https://img.shields.io/static/v1?label=node&message=%3E=14.16&logo=node.js&color)](https://nodejs.org/about/releases/)
[![Minimal npm version](https://img.shields.io/static/v1?label=npm&message=%3E=6.14.12&logo=npm&color)](https://github.com/npm/cli/releases)
[![Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https://GitHub.com/Naereen/StrapDown.js/graphs/commit-activity)
[![Linux](https://svgshare.com/i/Zhy.svg)](https://svgshare.com/i/Zhy.svg)
[![macOS](https://svgshare.com/i/ZjP.svg)](https://svgshare.com/i/ZjP.svg)
[![Visual Studio Code](https://img.shields.io/badge/--007ACC?logo=visual%20studio%20code&logoColor=ffffff)](https://code.visualstudio.com/)

# Eslint configuration

## Description

Eslint configuration for node & typescript

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

For example nodejs/js:

```json
{
  "scripts": {
    "lint": "eslint ."
  }
}
```

For example typescript:

```json
{
  "scripts": {
    "lint": "eslint . --ext .ts"
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

1. npm run lint:test - eslint test config
2. npm test - Run test with jest.
3. npm run lint - Lint your code.
4. npm run lint:fix - Lint & fix your code.
5. npm run release - Release library

## Docs

### Summary

- [library & tools](tools.md)

### Package maintenance

A modern cli tool that keeps your deps fresh

```bash
npx taze
```
