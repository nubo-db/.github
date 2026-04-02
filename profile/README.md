# nubo-db

Tooling for DynamoDB

## Dynoxide

A DynamoDB-compatible engine in Rust, backed by SQLite. Single binary, no JVM, no Docker. Starts in milliseconds. Runs as an HTTP server, an MCP server for coding agents, or embeds directly into applications as a library.

100% conformance across 526 tests validated against real DynamoDB.

- [dynoxide.dev](https://dynoxide.dev) - documentation and quick start
- [nubo-db/dynoxide](https://github.com/nubo-db/dynoxide) - source code
- [crates.io/crates/dynoxide-rs](https://crates.io/crates/dynoxide-rs) - Rust crate
- [npmjs.com/package/dynoxide](https://www.npmjs.com/package/dynoxide) - npm package (drop-in dynalite replacement)

```
brew install nubo-db/tap/dynoxide
```

## Nubo

Dynoxide was originally built as infrastructure for [Nubo](https://nubo.sinovi.uk); a native DynamoDB client for macOS and iPadOS, with Windows and Linux on the way. Nubo is a [Si Novi](https://sinovi.uk) product.

## DynamoDB Conformance Suite

An independent test suite for validating any DynamoDB-compatible endpoint against real DynamoDB behaviour. 526 tests across three tiers - core operations, advanced features, and strict validation. Works with DynamoDB, DynamoDB Local, Dynoxide, dynalite, LocalStack, or anything else that implements the DynamoDB HTTP API.

- [nubo-db/dynamodb-conformance](https://github.com/nubo-db/dynamodb-conformance) - source and results
