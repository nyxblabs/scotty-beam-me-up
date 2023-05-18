[![cover][cover-src]][cover-href]
[![npm version][npm-version-src]][npm-version-href] 
[![npm downloads][npm-downloads-src]][npm-downloads-href] 
[![bundle][bundle-src]][bundle-href] 
[![License][license-src]][license-href]

# 🛸 scotty-beam-me-up

> 🛸 Get an available TCP port to listen

[![npm version][npm-version-src]][npm-version-href]
[![npm downloads][npm-downloads-src]][npm-downloads-href]
[![License][license-src]][license-href]
[![JSDocs][jsdocs-src]][jsdocs-href]

## 💡 Usage

Install package:

```bash
npm i scotty-beam-me-up
```

```js
// ESM
import {
   checkPort,
   getPort,
   getRandomPort,
   waitForPort,
} from 'scotty-beam-me-up'

// CommonJS
const {
   getPort,
   checkPort,
   getRandomPort,
   waitForPort,
} = require('scotty-beam-me-up')
```

```ts
getPort(options?: GetPortOptions): Promise<number>
checkPort(port: number, host?: string): Promise<number | false>
waitForPort(port: number, options): Promise<number | false>
```

Try sequence is: port > ports > random

## 🎛️ Options

```ts
interface GetPortOptions {
   name?: string

   random?: boolean
   port?: number
   portRange?: [from: number, to: number]
   ports?: number[]
   host?: string

   memoDir?: string
   memoName?: string
}
```

### 📛 `name`

Unique name for port memorizing. Default is `default`.

### 🎲 `random`

If enabled, `port` and `ports` will be ignored. Default is `false`.

### ⚓️ `port`

First port to check. Default is `process.env.PORT || 3000`

### ⚓️⚓️ `ports`

Extended ports to check.

### 🔢 `portRange`

Extended port range to check.

### 🔢🔢 `alternativePortRange`

Alternative port range to check as fallback when non of the ports are available. Default is `[3000, 3100]` (only when `port` in unspecified.)

### 🏠 `host`

The host to check. Default is `process.env.HOST` otherwise all available hosts will be checked.

## 📜 License

[MIT](./LICENSE) - Made with 💞

<!-- Badges -->

[npm-version-src]: https://img.shields.io/npm/v/scotty-beam-me-up?style=flat&colorA=18181B&colorB=14F195
[npm-version-href]: https://npmjs.com/package/scotty-beam-me-up
[npm-downloads-src]: https://img.shields.io/npm/dm/scotty-beam-me-up?style=flat&colorA=18181B&colorB=14F195
[npm-downloads-href]: https://npmjs.com/package/scotty-beam-me-up
[bundle-src]: https://img.shields.io/bundlephobia/minzip/scotty-beam-me-up?style=flat&colorA=18181B&colorB=14F195
[bundle-href]: https://bundlephobia.com/result?p=scotty-beam-me-up
[license-src]: https://img.shields.io/github/license/nyxblabs/scotty-beam-me-up.svg?style=flat&colorA=18181B&colorB=14F195
[license-href]: https://github.com/nyxblabs/scotty-beam-me-up/blob/main/LICENSE

<!-- Cover -->
[cover-src]: https://raw.githubusercontent.com/nyxblabs/scotty-beam-me-up/main/.github/assets/cover-github-scotty-beam-me-up.png
[cover-href]: https://💻nyxb.ws
