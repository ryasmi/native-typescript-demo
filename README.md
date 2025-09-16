# Native TypeScript Demo
1. Run `nvm install` to install Node v22.18.
2. Run `npm t` to execute [`src/index.ts`](./src/index.ts).

## Supporting Info
https://nodejs.org/en/learn/typescript/run-natively

Since V22.6.0, Node.js has experimental support for some TypeScript syntax via "type stripping". You can write code that's valid TypeScript directly in Node.js without the need to transpile it first. The `--experimental-strip-types` flag tells Node.js to strip the type annotations from the TypeScript code before running it.

In V22.7.0 this experimental support was extended to transform TypeScript-only syntax, like enums and namespaces, with the addition of the `--experimental-transform-types` flag. Enabling `--experimental-transform-types` automatically implies that `--experimental-strip-types` is enabled, so there's no need to use both flags in the same command.

From v22.18.0 onwards, type stripping is enabled by default (you can disable it via `--no-experimental-strip-types`). However, running any code that requires transformations still needs the use of `--experimental-transform-types`.

https://blog.calm.com/engineering/how-we-migrated-our-rushjs-monorepo-to-node-type-stripping
