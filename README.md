# Repolex Knowledge Graph of samuelcolvin/pydantic-v2-startup-perf-bench

RDF knowledge graph data for [samuelcolvin/pydantic-v2-startup-perf-bench](https://github.com/samuelcolvin/pydantic-v2-startup-perf-bench), parsed by [repolex](https://repolex.ai).

> **Note**: This data is experimental and subject to change without notice.

## How to use this data

The easiest way to get started is to install the [rlex](https://github.com/repolex-ai/rlex) query tool:

```bash
cargo install --git https://github.com/repolex-ai/rlex
```

Verify the install:

```bash
rlex --help
```

**rlex is designed to be used primarily by LLMs in a terminal.** Start up your favorite AI assistant and ask it to use rlex. It handles the SPARQL — you just ask questions in plain English.

To load this repo's data:

```bash
rlex download samuelcolvin/pydantic-v2-startup-perf-bench
```

Consult `rlex --help` for other options, including SPARQL queries, HTTP server, and interactive visualization.

## Data structure

All data is stored as gzip-compressed [N-Quads](https://www.w3.org/TR/n-quads/) (`.nq.gz`), a standard RDF format that can be loaded into any triplestore or graph database.

```
.
├── aggregate
│   ├── ast
│   │   └── be3e0622078c2291d94b5ae9e6d41ee521f3de2d
│   │       └── chunk-001.nq.gz
│   └── repolex
│       └── be3e0622078c2291d94b5ae9e6d41ee521f3de2d
│           └── chunk-001.nq.gz
├── blob
│   ├── 00bfaf3e1c28b89c4d1119f6f0c3cecb661f88e2.nq.gz
│   ├── 0df5f29409545ed6cc657631e584b90de17f9297.nq.gz
│   ├── 193841d4fe0b2f996124906ad05ab0ef3c08f558.nq.gz
│   ├── 194e2db4a60ace79a8cd53034f1715a84f38589b.nq.gz
│   ├── 27f92a7aaf2418564bd95e3ef224446bbca93f74.nq.gz
│   ├── 371a3b364b1f939f97545676ef11d14b7d62e48e.nq.gz
│   ├── 3c8c56e3045915f1e587eb5a887f6787370caa7e.nq.gz
│   ├── 4ad603831390011d1980425f25a0e3fce58c5350.nq.gz
│   ├── 5105abacc8da6b69b758084e5357573dc92db7f1.nq.gz
│   ├── 5171940e32d34c5f79857050e526c9f99d3fb882.nq.gz
│   ├── 52118751b4fdf471238f51c454bdd7b39a949ed0.nq.gz
│   ├── 56fafb42f6e4c4cb25a31456163e355ffdca24c2.nq.gz
│   ├── 5e7eda97309d8f81d706227b28330d88835b3611.nq.gz
│   ├── 824da29d56ef07de1b50e8daf32cb3cf45e1c4a2.nq.gz
│   ├── 87ce1a9a5bb9ff1d5dbee45b66b0d56c9a89e494.nq.gz
│   ├── 8ab9980762f8d0f90375db05071b343c074010d1.nq.gz
│   ├── 8b137891791fe96927ad78e64b0aad7bded08bdc.nq.gz
│   ├── 8d7045167b629d4cc45bc4bc45e676d7a54b37c4.nq.gz
│   ├── 964a34d22ec512f183621e90dd838cfdaffb7df0.nq.gz
│   ├── bfe4a3653e9403a9b0afa48f0f6309ceb16ab5b7.nq.gz
│   ├── bff8f0f3994e39a0251b865451465db5990d88d9.nq.gz
│   ├── c6184ae0bed481fc9132320b5ad7c20d0093003a.nq.gz
│   ├── c66e698b65c33d111de3d83a00dcffb3886b5613.nq.gz
│   ├── c8cfe3959183f8e9a50f83f54cd723f2dc9c252d.nq.gz
│   ├── d18d417fd0056d1ad1a742086261ae9de5c4eece.nq.gz
│   ├── d356957ce54bccf5d551b18f927a7ef63a631459.nq.gz
│   ├── d5a75a76ce72ae123fe554749191d74f4bce12c3.nq.gz
│   ├── da132c8839914c8815cb1bc6015997036d172634.nq.gz
│   ├── e22611eae83922bb33ad28c30ae7a87ce0d8909c.nq.gz
│   ├── e69de29bb2d1d6434b8b29ae775ad8c2e48c5391.nq.gz
│   ├── fa3ef79ffc59680d3357c547f785f5aef3842532.nq.gz
│   └── fc6fd0d3c8a88339a237aeb881da4c0cd5891f35.nq.gz
├── branch
│   └── branch.nq.gz
├── commit
│   └── commit.nq.gz
├── filetree
│   └── be3e0622078c2291d94b5ae9e6d41ee521f3de2d.nq.gz
└── tag
    └── tag.nq.gz

11 directories, 38 files
```

| Directory | What it contains |
|-----------|-----------------|
| `blob/` | Per-file AST graphs, content-addressed by git blob SHA. Each file in the source repo gets its own graph. |
| `aggregate/ast/` | Combined AST graph per parsed commit. Merges all blob graphs for a snapshot of the entire codebase at that point. |
| `aggregate/lsp/` | Language Server Protocol enrichment: resolved symbols, definitions, references, and type information. |
| `aggregate/dataflow/` | Interprocedural data flow edges between functions and modules. |
| `aggregate/repolex/` | Combined graph (AST + LSP + dataflow) per commit. |
| `commit/` | Git commit metadata (author, date, message, parent links). |
| `branch/` | Branch metadata. |
| `tag/` | Tag metadata. |
| `filetree/` | File tree snapshots per commit (which files existed and their blob SHAs). |
| `audit/` | Code architecture and graph audit reports per commit. |

## Source repository

[samuelcolvin/pydantic-v2-startup-perf-bench](https://github.com/samuelcolvin/pydantic-v2-startup-perf-bench)

---
*Parsed on 2026-10-11 by [repolex](https://repolex.ai)*
