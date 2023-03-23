# @evan-yang/eslint-config

My ESLint config preset.

## Usage

### install

```sh
pnpm add -D eslint @evan-yang/eslint-config
```

### Config `.eslintrc`

```json
{
  "extends":"@evan-yang",
   "rules": {}
}
```

### Add script for package.json

```json
{
  "scripts": {
    "lint": "eslint .",
    "lint:fix": "eslint . --fix"
  }
}
```

### Auto Fix

`.vscode/settings.json`

```json
{
  "prettier.enable": false,
  "editor.codeActionsOnSave": {
    "source.fixAll.eslint": true
  }
}
```

## Packages

- eslint-config: default config preset
- eslint-plugin:
  - esnext: basic config
  - vue: vue support
  - react: react support
  - next: default config + next eslint config
  - json: parse json + package.json sort
  - yml: parse yml
  - typescript: typescript support
  - typescript-type-checking: typescript type checking


## Development

```bash
# install pnpm
npm i -g pnpm

# install deps
pnpm i

# run release script
pnpm release

# lint
pnpm lint
pnpm lint:fix
```

## License

MIT License © 2022 [mohen](https://github.com/yzh990918)
