# nubo-db

DynamoDB tooling.

## Dynoxide

A DynamoDB-compatible engine in Rust, backed by SQLite. Single binary, no JVM, no Docker. Starts in milliseconds. Run it as an HTTP server, an MCP server for coding agents, or embed it as a library.

100% conformance across 601 tests, validated against real DynamoDB.

Drop-in replacement for dynalite via npm:

```sh
npx dynoxide
```

Or with Homebrew:

```sh
brew install nubo-db/tap/dynoxide
```

- [dynoxide.dev](https://dynoxide.dev) - documentation and quick start
- [nubo-db/dynoxide](https://github.com/nubo-db/dynoxide) - source
- [crates.io/crates/dynoxide-rs](https://crates.io/crates/dynoxide-rs) - Rust crate
- [npmjs.com/package/dynoxide](https://www.npmjs.com/package/dynoxide) - npm package

## DynamoDB Conformance Suite

An independent test suite for validating any DynamoDB-compatible endpoint against real DynamoDB. 601 tests across three tiers - core operations, advanced features, and strict validation. Works with DynamoDB, DynamoDB Local, Dynoxide, dynalite, LocalStack, or anything that implements the DynamoDB HTTP API.

- [nubo-db/dynamodb-conformance](https://github.com/nubo-db/dynamodb-conformance) - source and results

## Nubo

Dynoxide started as infrastructure for [Nubo](https://nubo.sinovi.uk), a native DynamoDB client for macOS and iPadOS, with Windows and Linux on the way. Nubo is a [Si Novi](https://sinovi.uk) product.
