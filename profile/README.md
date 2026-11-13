# nubo-db

DynamoDB tooling from [Si Novi](https://sinovi.uk).

## Nubo

[Nubo](https://nubodb.com) is a native DynamoDB workspace for macOS, iPadOS, iOS, Android, Windows and Linux.

- **Explore** tables with Scan, Query, PartiQL or raw JSON, with request time and consumed capacity on every call. Backups, Streams, TTL and CloudWatch metrics sit alongside the data.
- **Model** single-table designs: entities detected from key prefixes or imported from OneTable, a relationship graph, a GSI builder with cost estimates, and access patterns turned into code.
- **Analyse** queries before they run - Nubo says whether a request will be a GetItem, Query or Scan.
- **Bring your agent** - Claude Code, Cursor, VS Code or Claude Desktop can ask Nubo to open a query. You approve it, it opens read-only, and you choose which rows go back.

Nubo connects to AWS DynamoDB with profiles, SSO and MFA, and to DynamoDB Local, LocalStack, Dynoxide or any compatible endpoint. Its built-in sandbox runs on Dynoxide and is free forever, with no account needed.

Nubo is in closed beta. [Join the waitlist](https://nubodb.com/#signup).

## Dynoxide

A DynamoDB-compatible engine in Rust, backed by SQLite. Single binary, no JVM, no Docker. Starts in milliseconds. Run it as an HTTP server, an MCP server for coding agents, or embed it as a library. It is the engine behind Nubo's sandbox.

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
