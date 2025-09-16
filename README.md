# Native TypeScript Demo
Run with `npm t`

## Supporting Info
https://nodejs.org/en/learn/typescript/run-natively

In V22.7.0 this experimental support was extended to transform TypeScript-only syntax, like enums and namespaces, with the addition of the `--experimental-transform-types` flag. Enabling `--experimental-transform-types` automatically implies that `--experimental-strip-types` is enabled, so there's no need to use both flags in the same command.

From v22.18.0 onwards, type stripping is enabled by default (you can disable it via `--no-experimental-strip-types`). However, running any code that requires transformations still needs the use of `--experimental-transform-types`.
