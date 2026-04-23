# Repolex Knowledge Graph of near/near-api-rs

RDF knowledge graph data for [near/near-api-rs](https://github.com/near/near-api-rs), parsed by [repolex](https://repolex.ai).

> **Note**: This data is experimental and subject to change without notice.

## How to use this data

The easiest way to get started is to install the [lexq](https://github.com/repolex-ai/lexq) query tool using [uv](https://docs.astral.sh/uv/getting-started/installation/).

If you have uv installed, just copy/paste this into your terminal:

```bash
uv tool install git+https://github.com/repolex-ai/lexq
```

This installs lexq onto your system, in your user context. Verify the install:

```bash
lexq --help
```

**lexq is designed to be used primarily by LLMs in a terminal.** Start up your favorite LLM and ask it to use the lexq tool. It's that easy!

To load this repo's data:

```bash
lexq download near/near-api-rs
```

This will automatically download essential data files from the last parsed commit. Consult `lexq --moreinfo` for other options, including downloading multiple commits, blobs, etc.

## Data structure

All data is stored as gzip-compressed [N-Quads](https://www.w3.org/TR/n-quads/) (`.nq.gz`), a standard RDF format that can be loaded into any triplestore or graph database.

```
.
├── aggregate
│   ├── ast
│   │   └── 9bb44009e187fc8ce5fd5b9366a026ea01a4b9c6
│   │       └── chunk-001.nq.gz
│   ├── lsp
│   │   └── 9bb44009e187fc8ce5fd5b9366a026ea01a4b9c6.nq.gz
│   └── repolex
│       └── 9bb44009e187fc8ce5fd5b9366a026ea01a4b9c6
│           └── chunk-001.nq.gz
├── blob
│   ├── 000ca066bc6a7a69bfa72111b4a32893efc895af.nq.gz
│   ├── 03d61301d75144729529aac2228d53cbe0e2079f.nq.gz
│   ├── 06988f70d81fa33ba546edc7d1f3f9953b02dc2f.nq.gz
│   ├── 0e52542130a761bf130022f620b2e8fe20a981c5.nq.gz
│   ├── 1b3f2a0ad45f7e11b97492312396c24c627c0e1f.nq.gz
│   ├── 1deb83060045e92e8326cc6b2593c33d2729e98d.nq.gz
│   ├── 230f24b19441bfc1e44cad7a6e1749a91af730e2.nq.gz
│   ├── 261e555f44cbbf2c109a21c8677ec11ccdce9ea8.nq.gz
│   ├── 296fed842240fbc4eecbe91f0a97d5030674014f.nq.gz
│   ├── 305ad08ebb8c495734fdfb6fac678b8ae05c2741.nq.gz
│   ├── 3375f9e876cef1041cf4ab7e5696853cd7a6f3ae.nq.gz
│   ├── 36929c3c31221d0a63abf92d00c8a681b4d22537.nq.gz
│   ├── 3c9328a954a9e1b7cde5837493b29aed7f30e758.nq.gz
│   ├── 3e9655208d9c4abc6ded1b2c37f31bdb41d8f98e.nq.gz
│   ├── 49ec673677103e3c7cf40c62042b5003670ee55d.nq.gz
│   ├── 4fcec0b5c2319a019e3ed478c7c134b08000ff71.nq.gz
│   ├── 53533e59fd071feee2f313bda584f7ca86bd269d.nq.gz
│   ├── 538423ca33a78d7b5c732373218c719828a45331.nq.gz
│   ├── 57206a785518b0750d1885506544dc1acee3d898.nq.gz
│   ├── 6060464ead6909b1c9a76cc497da305e69e226fe.nq.gz
│   ├── 66dd75ab4b323de1918b30bc78b2b332aab059bf.nq.gz
│   ├── 6a05df63178019c3e23586e398f435fa59634c56.nq.gz
│   ├── 6ba1022c564813bbe2ebb215c8515305157fe6d2.nq.gz
│   ├── 6f44d6ce2356e22e206fc8e2cfc163934ae4621f.nq.gz
│   ├── 719ff53cf661ef7bbd6df611cf170c59dcf7225a.nq.gz
│   ├── 72dc60d84b692387206266939bc34656bcba1e15.nq.gz
│   ├── 74b7437c527b989e3a4cb6dcca14d09fa553de24.nq.gz
│   ├── 74f1b60279460575b582ebb7b568d38df4050a52.nq.gz
│   ├── 77d91ef59be99905df2bc1a569a4df11c0a8cef7.nq.gz
│   ├── 7c145167277d10ad455f0f7a14508ca163f53343.nq.gz
│   ├── 80363bd962d7ee2d9a1e9434f2ebeeec0e688b13.nq.gz
│   ├── 8c967c36df65ad6995a7337ad48ae830cbeebf93.nq.gz
│   ├── 8d74646580be8e9efe08e93014c45f35c9a322fd.nq.gz
│   ├── 8f036e1a0fb4898870f9639cc44df2f223b2b902.nq.gz
│   ├── 8f43af573a005f47a81e41de66cde601dba1c284.nq.gz
│   ├── a360c210cbf16f9c56409c91f27e028f42cadc30.nq.gz
│   ├── a74c0348b7ca87cac4f431d69f65766d40168fff.nq.gz
│   ├── aaa40a0ed7c4ad957833b088bb8b9570793c9386.nq.gz
│   ├── abe0a7b01e766b9ff65609dd6616c35deb29cdcb.nq.gz
│   ├── b77ac64db4f43fd2d7d0929bd10ec823926376bc.nq.gz
│   ├── c96ade41f59a755def5bf7482cb96b026c92273c.nq.gz
│   ├── ca519dca8d4f0c5fe33c395e2599d561337acf3f.nq.gz
│   ├── cbdcd16b84e9070cb6c11d2495b398a2d5edd646.nq.gz
│   ├── ce74479dc10d68bc1b1669482fa56a78dc14147b.nq.gz
│   ├── ceaa0191bf3a1fc6463356f29f123b1966d0a500.nq.gz
│   ├── cee533256369f1f5ad1992a72731a425c6b3dfdf.nq.gz
│   ├── d04ad7c49dd507c4dee94530cce5d52bf89e1ce0.nq.gz
│   ├── d0a78455ca86857c4825a73a9291a27422365293.nq.gz
│   ├── d29dcecb2b21b0f1f37c0c380d853d880045a3e7.nq.gz
│   ├── d52898a494d25918bc06f072974f21b6433f9b1d.nq.gz
│   ├── d717aae48f07a70db1510ce7b98a9e2dc9c8e80e.nq.gz
│   ├── dbc6aca11e92cb2f9244b285847a0ca0b3ed7a4d.nq.gz
│   ├── e07c8f17d174b161264e7cb0876ea3e73a99ca41.nq.gz
│   ├── e08d35757667a6775c268b889d24c11f7760b11b.nq.gz
│   ├── e0f4ab4af770df0f8a4e4f0c26adc07e93b838d9.nq.gz
│   ├── e79e011b2bc950a744358bc22c5bcd25d0d92c89.nq.gz
│   ├── efd44bb63798e90686f63e0ee7587f5795ffc4dd.nq.gz
│   └── f061a3c308dc9744b792967ebe723c1739fa18c9.nq.gz
├── branch
│   └── branch.nq.gz
├── commit
│   └── commit.nq.gz
├── dep
│   └── 9bb44009e187fc8ce5fd5b9366a026ea01a4b9c6.nq.gz
├── filetree
│   └── 9bb44009e187fc8ce5fd5b9366a026ea01a4b9c6.nq.gz
├── issue
│   └── issue.nq.gz
├── pr
│   └── pr.nq.gz
└── tag
    └── tag.nq.gz

15 directories, 68 files
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

## Source repository

[near/near-api-rs](https://github.com/near/near-api-rs)

---
*Parsed on 2026-04-23 by [repolex](https://repolex.ai)*
