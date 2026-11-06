# Repolex Knowledge Graph of ansible-community/stats-container-meetups

RDF knowledge graph data for [ansible-community/stats-container-meetups](https://github.com/ansible-community/stats-container-meetups), parsed by [repolex](https://repolex.ai).

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
rlex download ansible-community/stats-container-meetups
```

Consult `rlex --help` for other options, including SPARQL queries, HTTP server, and interactive visualization.

## Data structure

All data is stored as gzip-compressed [N-Quads](https://www.w3.org/TR/n-quads/) (`.nq.gz`), a standard RDF format that can be loaded into any triplestore or graph database.

```
.
├── aggregate
│   ├── ast
│   │   └── 557442414ed4f3e618a6e3c07a7ff867a8dadd44
│   │       └── chunk-001.nq.gz
│   └── repolex
│       └── 557442414ed4f3e618a6e3c07a7ff867a8dadd44
│           └── chunk-001.nq.gz
├── blob
│   ├── 0c870c121d1a21fd484c151d63d51fb08e9a7b19.nq.gz
│   ├── 16cd0f759bb037c9e14a882182987a57dac8a77e.nq.gz
│   ├── 1fa3986bbc93f2bddb7c23d6fc9a34501947a6f6.nq.gz
│   ├── 22a1dafaf806225fc43caece8349082b1fd0ab03.nq.gz
│   ├── 2dbc2e6372dd82692ef558518e4ee5930dcf03be.nq.gz
│   ├── 2e2d3329302acc17a390b7bf2db7d0361149d043.nq.gz
│   ├── 334ae1074affe7df4916bce577cb8a5aeabc3a89.nq.gz
│   ├── 4afde63e99e090d1fb76545974a1e6da8af6472a.nq.gz
│   ├── 7d554571f9860ba4fdb1f6de8cae10ca90e45c2a.nq.gz
│   ├── 96fcd7e5dae1942767365474e4efeadca8309afe.nq.gz
│   ├── 99a44d6e6109df14e472f57bdbb7f32c9040dc0d.nq.gz
│   ├── a7a7213dba99530da166a279d7023d082d549081.nq.gz
│   ├── b4d90790223b95552556ea895ac541a489a7379d.nq.gz
│   ├── c9ec7ad9bb931690121c4b7a721d82da18419bd7.nq.gz
│   ├── de2fc14efa82a42d1125af64da5a4e3fd8b4468f.nq.gz
│   ├── e69de29bb2d1d6434b8b29ae775ad8c2e48c5391.nq.gz
│   └── f288702d2fa16d3cdf0035b15a9fcbc552cd88e7.nq.gz
├── branch
│   └── branch.nq.gz
├── commit
│   └── commit.nq.gz
├── filetree
│   └── 557442414ed4f3e618a6e3c07a7ff867a8dadd44.nq.gz
├── pr
│   └── pr.nq.gz
└── tag
    └── tag.nq.gz

12 directories, 24 files
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

[ansible-community/stats-container-meetups](https://github.com/ansible-community/stats-container-meetups)

---
*Parsed on 2026-11-06 by [repolex](https://repolex.ai)*
