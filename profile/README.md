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

A DynamoDB emulator in Rust, backed by SQLite. Single binary, no JVM, no Docker. Starts in milliseconds. Run it as an HTTP server or an MCP server for coding agents, embed it in Rust and iOS apps as a library, or compile it to WebAssembly for the browser. It is the engine behind Nubo's sandbox.

Dynoxide is scored continuously against real DynamoDB by [Parity Suite](https://paritysuite.org) - see the live standings for its current results.

Run it without installing anything:

```sh
npx dynoxide
```

Or with Docker, as a drop-in for `amazon/dynamodb-local`:

```sh
docker run --rm -p 8000:8000 ghcr.io/nubo-db/dynoxide
```

Or with Homebrew:

```sh
brew install nubo-db/tap/dynoxide
```

- [dynoxide.dev](https://dynoxide.dev) - documentation and quick start
- [nubo-db/dynoxide](https://github.com/nubo-db/dynoxide) - source
- [crates.io/crates/dynoxide-rs](https://crates.io/crates/dynoxide-rs) - Rust crate
- [npmjs.com/package/dynoxide](https://www.npmjs.com/package/dynoxide) - npm package

## Parity Suite

An independent conformance suite that validates any DynamoDB-compatible endpoint against real DynamoDB, across three tiers - core operations, complete features and strict validation. It scores DynamoDB Local, LocalStack, Dynoxide, Dynalite and other emulators on the same matrix, with live results tracked run over run. Parity Suite is maintained by the same person as Dynoxide, and its tests and results are open.

- [paritysuite.org](https://paritysuite.org) - live standings
- [paritysuite/dynamodb-conformance](https://github.com/paritysuite/dynamodb-conformance) - source and results
