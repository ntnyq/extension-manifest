# vscode-extension-manifest

[![CI](https://github.com/ntnyq/vscode-extension-manifest/workflows/CI/badge.svg)](https://github.com/ntnyq/vscode-extension-manifest/actions)
[![NPM VERSION](https://img.shields.io/npm/v/vscode-extension-manifest.svg)](https://www.npmjs.com/package/vscode-extension-manifest)
[![NPM DOWNLOADS](https://img.shields.io/npm/dy/vscode-extension-manifest.svg)](https://www.npmjs.com/package/vscode-extension-manifest)
[![CODECOV](https://codecov.io/github/ntnyq/vscode-extension-manifest/branch/main/graph/badge.svg)](https://codecov.io/github/ntnyq/vscode-extension-manifest)
[![LICENSE](https://img.shields.io/github/license/ntnyq/vscode-extension-manifest.svg)](https://github.com/ntnyq/vscode-extension-manifest/blob/main/LICENSE)

> VSCode extension manifest type definitions.

## Install

```shell
npm install vscode-extension-manifest -D
```

```shell
yarn add vscode-extension-manifest -D
```

```shell
pnpm add vscode-extension-manifest -D
```

## Usage

```ts
import { readExtensionManifest } from 'vscode-extension-manifest'

console.log(await readExtensionManifest())
//=> VSCode extension manifest with types definition
```

## API

### readExtensionManifest

Returns a `Promise` for VSCode extension manifest with type definition.

### readExtensionManifestSync

Returns the VSCode extension manifest with type definition.

### validateExtensionManifest

Returns `true` if the extension manifest is valid, `false` otherwise.

By checking the following properties:

- `publisher`

## Parameters

for `readExtensionManifest` and `readExtensionManifestSync`

### filename

- Type: `string | URL`
- Default: `package.json`

The filename of the extension manifest.

### cwd

- Type: `string`
- Default: `process.cwd()`

The current working directory of the extension manifest.

## Links

- [Extension Manifest](https://code.visualstudio.com/api/references/extension-manifest)
- [Contribution Points](https://code.visualstudio.com/api/references/contribution-points)

## License

[MIT](./LICENSE) License © 2024-PRESENT [ntnyq](https://github.com/ntnyq)