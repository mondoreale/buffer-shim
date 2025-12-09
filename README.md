# buffer-shim 🧱

A tiny shim that installs the [`buffer`](https://www.npmjs.com/package/buffer) module onto `globalThis.Buffer`.
Useful in runtimes or bundlers where `Buffer` is not provided by default.

## How it works

`buffer-shim` takes the `buffer` npm module (declared as a peer dependency) and exposes it globally so your code — or third-party libraries — can rely on `Buffer` without additional setup.

## Install

```bash
npm i buffer buffer-shim
```

## Usage

```ts
import 'buffer-shim';

// Now globalThis.Buffer is available
const b = Buffer.from('hello');
```

## License

MIT
