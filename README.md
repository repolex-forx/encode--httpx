# Repolex Knowledge Graph of encode/httpx

RDF knowledge graph data for [encode/httpx](https://github.com/encode/httpx), parsed by [repolex](https://repolex.ai).

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
lexq download encode/httpx
```

This will automatically download essential data files from the last parsed commit. Consult `lexq --moreinfo` for other options, including downloading multiple commits, blobs, etc.

## Data structure

All data is stored as gzip-compressed [N-Quads](https://www.w3.org/TR/n-quads/) (`.nq.gz`), a standard RDF format that can be loaded into any triplestore or graph database.

```
.
├── aggregate
│   ├── ast
│   │   ├── 07f786c2f871d230f9c93b5f351b4aa305ee1599.nq.gz
│   │   ├── 08a557e3e2b9220b90ee21238e316206ffa65d36.nq.gz
│   │   ├── 08eff926a6011ac84961fd2cee22d9fd4d4b1a88.nq.gz
│   │   ├── 0d7c4caada43324cb3b6ebe4101745c0f7f575db.nq.gz
│   │   ├── 15c51b9dd5dfe3ede3d8c2de72073e3a678ff5a2.nq.gz
│   │   ├── 23486b5438c8c142c430aba702d61144ec2e901b.nq.gz
│   │   ├── 26d48e0634e6ee9cdc0533996db289ce4b430177.nq.gz
│   │   ├── 35164b7a64fbda91629778f37f05afd6ac3f17ee.nq.gz
│   │   ├── 35b7516674ced88073eace33b5d58c4c4d6bab65.nq.gz
│   │   ├── 56d880030e37d64c273ea23b92e24dc00b586c3b.nq.gz
│   │   ├── 609df7ecc0f7cb10a1c998aa9c269bba77337c5f.nq.gz
│   │   ├── 66594e30dc733dd47724a540f7efb8e0208991ee.nq.gz
│   │   ├── 75b8fa4d0d62ce459f5c8aaff539f5c7528152e5.nq.gz
│   │   ├── 77cf336eabcd53fbbda0c69dc692b5df820f578c.nq.gz
│   │   ├── 831e79f50a59cb7c2af549fc186951703497fe08.nq.gz
│   │   ├── 91a2a1b8968bceae16e3cdcbae396dd212cdf7da.nq.gz
│   │   ├── 92ca4d0cc654859fc2257c492e55d8752370d427.nq.gz
│   │   ├── 9904684d353f8d806755918533487b78138f7c08.nq.gz
│   │   ├── 9f192bbf0bb62d801bfe9a78d01f7ba1580c3469.nq.gz
│   │   ├── a5f99830376ead8d7a1357169f49d9c76f085622.nq.gz
│   │   ├── b128bfaf211314dfb9b0a19ab6e00cfbe98522b8.nq.gz
│   │   ├── b5addb64f0161ff6bfe94c124ef76f6a1fba5254.nq.gz
│   │   ├── ba033c549f5c2834e7ebc79739a86d84dad86d62.nq.gz
│   │   ├── c9354282ba60a857f959e5fe60cdf2b74cdbd294.nq.gz
│   │   ├── cc206cf2dad42600479962ac1daaa44675cfaf56.nq.gz
│   │   ├── e05a5372eb6172287458b37447c30f650047e1b8.nq.gz
│   │   ├── ec06ba244e0a59e3152491c7899713222ebd7ac6.nq.gz
│   │   ├── f312e629bf0f1a03ae66bc08130e2fb0799a1c89.nq.gz
│   │   ├── f4591f08ae0a8009789ff23a68cb1830ea7100f5.nq.gz
│   │   └── fcf1bc73dbe13bc61d18a6e998237a5021d3341c.nq.gz
│   ├── dataflow
│   │   ├── 07f786c2f871d230f9c93b5f351b4aa305ee1599.nq.gz
│   │   ├── 08a557e3e2b9220b90ee21238e316206ffa65d36.nq.gz
│   │   ├── 08eff926a6011ac84961fd2cee22d9fd4d4b1a88.nq.gz
│   │   ├── 0d7c4caada43324cb3b6ebe4101745c0f7f575db.nq.gz
│   │   ├── 15c51b9dd5dfe3ede3d8c2de72073e3a678ff5a2.nq.gz
│   │   ├── 23486b5438c8c142c430aba702d61144ec2e901b.nq.gz
│   │   ├── 26d48e0634e6ee9cdc0533996db289ce4b430177.nq.gz
│   │   ├── 35164b7a64fbda91629778f37f05afd6ac3f17ee.nq.gz
│   │   ├── 35b7516674ced88073eace33b5d58c4c4d6bab65.nq.gz
│   │   ├── 56d880030e37d64c273ea23b92e24dc00b586c3b.nq.gz
│   │   ├── 609df7ecc0f7cb10a1c998aa9c269bba77337c5f.nq.gz
│   │   ├── 66594e30dc733dd47724a540f7efb8e0208991ee.nq.gz
│   │   ├── 75b8fa4d0d62ce459f5c8aaff539f5c7528152e5.nq.gz
│   │   ├── 77cf336eabcd53fbbda0c69dc692b5df820f578c.nq.gz
│   │   ├── 831e79f50a59cb7c2af549fc186951703497fe08.nq.gz
│   │   ├── 91a2a1b8968bceae16e3cdcbae396dd212cdf7da.nq.gz
│   │   ├── 92ca4d0cc654859fc2257c492e55d8752370d427.nq.gz
│   │   ├── 9904684d353f8d806755918533487b78138f7c08.nq.gz
│   │   ├── 9f192bbf0bb62d801bfe9a78d01f7ba1580c3469.nq.gz
│   │   ├── a5f99830376ead8d7a1357169f49d9c76f085622.nq.gz
│   │   ├── b128bfaf211314dfb9b0a19ab6e00cfbe98522b8.nq.gz
│   │   ├── b5addb64f0161ff6bfe94c124ef76f6a1fba5254.nq.gz
│   │   ├── ba033c549f5c2834e7ebc79739a86d84dad86d62.nq.gz
│   │   ├── c9354282ba60a857f959e5fe60cdf2b74cdbd294.nq.gz
│   │   ├── cc206cf2dad42600479962ac1daaa44675cfaf56.nq.gz
│   │   ├── e05a5372eb6172287458b37447c30f650047e1b8.nq.gz
│   │   ├── ec06ba244e0a59e3152491c7899713222ebd7ac6.nq.gz
│   │   ├── f312e629bf0f1a03ae66bc08130e2fb0799a1c89.nq.gz
│   │   ├── f4591f08ae0a8009789ff23a68cb1830ea7100f5.nq.gz
│   │   └── fcf1bc73dbe13bc61d18a6e998237a5021d3341c.nq.gz
│   ├── lsp
│   │   ├── 07f786c2f871d230f9c93b5f351b4aa305ee1599.nq.gz
│   │   ├── 08a557e3e2b9220b90ee21238e316206ffa65d36.nq.gz
│   │   ├── 08eff926a6011ac84961fd2cee22d9fd4d4b1a88.nq.gz
│   │   ├── 0d7c4caada43324cb3b6ebe4101745c0f7f575db.nq.gz
│   │   ├── 15c51b9dd5dfe3ede3d8c2de72073e3a678ff5a2.nq.gz
│   │   ├── 23486b5438c8c142c430aba702d61144ec2e901b.nq.gz
│   │   ├── 26d48e0634e6ee9cdc0533996db289ce4b430177.nq.gz
│   │   ├── 35164b7a64fbda91629778f37f05afd6ac3f17ee.nq.gz
│   │   ├── 35b7516674ced88073eace33b5d58c4c4d6bab65.nq.gz
│   │   ├── 56d880030e37d64c273ea23b92e24dc00b586c3b.nq.gz
│   │   ├── 609df7ecc0f7cb10a1c998aa9c269bba77337c5f.nq.gz
│   │   ├── 66594e30dc733dd47724a540f7efb8e0208991ee.nq.gz
│   │   ├── 75b8fa4d0d62ce459f5c8aaff539f5c7528152e5.nq.gz
│   │   ├── 77cf336eabcd53fbbda0c69dc692b5df820f578c.nq.gz
│   │   ├── 831e79f50a59cb7c2af549fc186951703497fe08.nq.gz
│   │   ├── 91a2a1b8968bceae16e3cdcbae396dd212cdf7da.nq.gz
│   │   ├── 92ca4d0cc654859fc2257c492e55d8752370d427.nq.gz
│   │   ├── 9904684d353f8d806755918533487b78138f7c08.nq.gz
│   │   ├── 9f192bbf0bb62d801bfe9a78d01f7ba1580c3469.nq.gz
│   │   ├── a5f99830376ead8d7a1357169f49d9c76f085622.nq.gz
│   │   ├── b128bfaf211314dfb9b0a19ab6e00cfbe98522b8.nq.gz
│   │   ├── b5addb64f0161ff6bfe94c124ef76f6a1fba5254.nq.gz
│   │   ├── ba033c549f5c2834e7ebc79739a86d84dad86d62.nq.gz
│   │   ├── c9354282ba60a857f959e5fe60cdf2b74cdbd294.nq.gz
│   │   ├── cc206cf2dad42600479962ac1daaa44675cfaf56.nq.gz
│   │   ├── e05a5372eb6172287458b37447c30f650047e1b8.nq.gz
│   │   ├── ec06ba244e0a59e3152491c7899713222ebd7ac6.nq.gz
│   │   ├── f312e629bf0f1a03ae66bc08130e2fb0799a1c89.nq.gz
│   │   ├── f4591f08ae0a8009789ff23a68cb1830ea7100f5.nq.gz
│   │   └── fcf1bc73dbe13bc61d18a6e998237a5021d3341c.nq.gz
│   └── repolex
│       ├── 07f786c2f871d230f9c93b5f351b4aa305ee1599.nq.gz
│       ├── 08a557e3e2b9220b90ee21238e316206ffa65d36.nq.gz
│       ├── 08eff926a6011ac84961fd2cee22d9fd4d4b1a88.nq.gz
│       ├── 0d7c4caada43324cb3b6ebe4101745c0f7f575db.nq.gz
│       ├── 15c51b9dd5dfe3ede3d8c2de72073e3a678ff5a2.nq.gz
│       ├── 23486b5438c8c142c430aba702d61144ec2e901b.nq.gz
│       ├── 26d48e0634e6ee9cdc0533996db289ce4b430177.nq.gz
│       ├── 35164b7a64fbda91629778f37f05afd6ac3f17ee.nq.gz
│       ├── 35b7516674ced88073eace33b5d58c4c4d6bab65.nq.gz
│       ├── 56d880030e37d64c273ea23b92e24dc00b586c3b.nq.gz
│       ├── 609df7ecc0f7cb10a1c998aa9c269bba77337c5f.nq.gz
│       ├── 66594e30dc733dd47724a540f7efb8e0208991ee.nq.gz
│       ├── 75b8fa4d0d62ce459f5c8aaff539f5c7528152e5.nq.gz
│       ├── 77cf336eabcd53fbbda0c69dc692b5df820f578c.nq.gz
│       ├── 831e79f50a59cb7c2af549fc186951703497fe08.nq.gz
│       ├── 91a2a1b8968bceae16e3cdcbae396dd212cdf7da.nq.gz
│       ├── 92ca4d0cc654859fc2257c492e55d8752370d427.nq.gz
│       ├── 9904684d353f8d806755918533487b78138f7c08.nq.gz
│       ├── 9f192bbf0bb62d801bfe9a78d01f7ba1580c3469.nq.gz
│       ├── a5f99830376ead8d7a1357169f49d9c76f085622.nq.gz
│       ├── b128bfaf211314dfb9b0a19ab6e00cfbe98522b8.nq.gz
│       ├── ba033c549f5c2834e7ebc79739a86d84dad86d62.nq.gz
│       ├── c9354282ba60a857f959e5fe60cdf2b74cdbd294.nq.gz
│       ├── cc206cf2dad42600479962ac1daaa44675cfaf56.nq.gz
│       ├── e05a5372eb6172287458b37447c30f650047e1b8.nq.gz
│       ├── ec06ba244e0a59e3152491c7899713222ebd7ac6.nq.gz
│       ├── f312e629bf0f1a03ae66bc08130e2fb0799a1c89.nq.gz
│       ├── f4591f08ae0a8009789ff23a68cb1830ea7100f5.nq.gz
│       └── fcf1bc73dbe13bc61d18a6e998237a5021d3341c.nq.gz
└── blob
    ├── 00913b2c17dbc7c0eab7aa3379b1ce4b19c4ca10.nq.gz
    ├── 00935fb421e64564ba0d9983cf3b9cddf360af8a.nq.gz
    ├── 00e0a7e4fcddd42e9051193e1c37ef42e1c89f7a.nq.gz
    ├── 012d2b747fa1e2caed2853d0c72ae29aedb47116.nq.gz
    ├── 0134bee854f44b2cfc0d41e903963393d6b29356.nq.gz
    ├── 016c15a7e60ef003cbf1cca0f68c16094f939200.nq.gz
    ├── 017eae18df66851f216155e2e90aff96f7157d5f.nq.gz
    ├── 0187eec47ef4e49d420c71d3b13e69ed0c9dd824.nq.gz
    ├── 018d1a99aeb7f904306a28f58dbed7fc2e615fdd.nq.gz
    ├── 019876e43e883cdf659fbdf5350458d8c0710bd2.nq.gz
    ├── 01aaa7db466e8f9e147b86cc0f4538745e64b73b.nq.gz
    ├── 01c1aae13db8ed62cb9c448b8e7f41d005a31768.nq.gz
    ├── 01d0de828403d28b5a539443716c8e47609205e0.nq.gz
    ├── 01d9583bc5edd0e16fa1e8eadddd32e6039d762f.nq.gz
    ├── 01f458532f0d7c39d949ea9a6e98096131725fcc.nq.gz
    ├── 02460fd3b1257d2f15ddb89abe6775e30327536b.nq.gz
    ├── 02487683233611fbeaadaea3e91da747b1836f9b.nq.gz
    ├── 02a00e70a1053993d733f0eb86e6c73f6e268a39.nq.gz
    ├── 02ccc86a03522e8ce3cd716ef5d1e5c91d00d326.nq.gz
    ├── 0303d74562872a92a7467d043df816c4be8c669c.nq.gz
    ├── 03072e8f5cdb5314ceab580c664d0c890949a365.nq.gz
    ├── 0347d3124cd7a82dfb9b375b0870834b93ff7d81.nq.gz
    ├── 0364deb0613477a82f40055244f307fbd5b24e76.nq.gz
    ├── 04a9a2e66005996c5dad532e9f7f8ca0714875c9.nq.gz
    ├── 053ad289ccdb1282931f2fa78abfe5f19c4302ce.nq.gz
    ├── 0573c9cf4ccfe4c8add89c83e7a841bd3d3837a0.nq.gz
    ├── 058691a30e8674bc7f4295473ea0d417c447873f.nq.gz
    ├── 05c096dfc3103aec8971ce406c9aaee0155ba283.nq.gz
    ├── 064c25a64559e688ade1467cd70446bd1923f237.nq.gz
    ├── 068547ffc99518d81e5b9d6f02dd47b03a907f81.nq.gz
    ├── 06c28e1e30b3bb77325327e82b368687f6bbe65c.nq.gz
    ├── 06ebb92c42ad391ce100d8351510c68efe0640c2.nq.gz
    ├── 072db3f1e8a345db11e790a1326b659168e18af1.nq.gz
    ├── 075673ee6f02a7c71a30fbbccc1b4d350d79c41b.nq.gz
    ├── 07b0229bfa6999de0f1876c1e7375292dff84d82.nq.gz
    ├── 07bbea9070cc6451c33f8cec7bcb0e607f25b000.nq.gz
    ├── 07be1f13cc7e5e60cb394c891dd0fadfebd80a30.nq.gz
    ├── 07ff750d49846da95b6fe3b731b3f88bb92fa720.nq.gz
    ├── 089d7831915c0b465d0da7de21523e1723cacfa3.nq.gz
    ├── 08cd392f75c62b3d6aa9ee547ed9e6fc4fd702d0.nq.gz
    ├── 0995c7fa001f91bf6c10d640a57b9426ab3c3b92.nq.gz
    ├── 09b25160e76cacbf0298a39104f23f734567df38.nq.gz
    ├── 09e5953c9d881bf57690673db08fca95a0ef5c93.nq.gz
    ├── 0aaea33749a3d1ce41578c2ced4cce7d006c4b0f.nq.gz
    ├── 0b0101cb310d97d1fbb4bf1f4acbf74ad4ac8c4e.nq.gz
    ├── 0b14734d2868ee86cb4a42f11a1be2616ecc0155.nq.gz
    ├── 0b8ef00bea74b6a90e3bcfa6355b5ce0628c5635.nq.gz
    ├── 0bb570cedb51dbc57b08f097523c5e9aa245f854.nq.gz
    ├── 0be86184779dd30f9217f0b4f03e97f013ea26ce.nq.gz
    ├── 0c0971c92479f634872de097e4b192ed8501fed6.nq.gz
    ├── 0c1d3409eb8152ea2fbeb49e9ece0762ccbbae93.nq.gz
    ├── 0c303e462589300bc7fccf9a75c0a064845b86f4.nq.gz
    ├── 0c64988dbee852fe2f76ed862fe19acced54c80d.nq.gz
    ├── 0c8c9177be65f96e3183ded1a619b4a7cdb5a228.nq.gz
    ├── 0d7d1350831a8f4e153454c158a4a7cb2d7ab5c1.nq.gz
    ├── 0d8ba2eff0a6cdbc70527910cea1bd4d92fc20ed.nq.gz
    ├── 0daa78c610c403f4190bcd5c0b4f65aa9302610d.nq.gz
    ├── 0dcf99535dc23a7c5a9623548aaf07b6ab1f2376.nq.gz
    ├── 0ddd8c85b6c6c2e544b929a3e09813a1001f689e.nq.gz
    ├── 0e83ebf6a17ebb5815c992730b9d16e5dc87f17c.nq.gz
    ├── 0eeb32d145a09574cde20766200161a784972ad2.nq.gz
    ├── 0f0ea062d32e251da98cc8a2b9fc73eddd4f7c59.nq.gz
    ├── 0f1b2864ffb2d3fa49ebfc28069d1e6ef85b3d30.nq.gz
    ├── 0f83eddd7ffd78daaccada9008d3de687ac8bb2c.nq.gz
    ├── 100aec641bf9e17942073562258aa33aa0fbf100.nq.gz
    ├── 110a127c7459b129e16b7b9514d7cfc111c12116.nq.gz
    ├── 1138c30c56b0c4bb2ec4dbacc99d157537b849ef.nq.gz
    ├── 123692955b10426a8d45cfb45b7c6ff2d7578417.nq.gz
    ├── 123a890847fa202abdc7ff143e5703b7211b2f3a.nq.gz
    ├── 126c50e95bec93e392233a4423b6122598b2cb9d.nq.gz
    ├── 129780642ef5a5da43ccedcf5b3d81fd9fa59a92.nq.gz
    ├── 12b790af96fef2bfd7948305dfad4ad98cb3c437.nq.gz
    ├── 12d0fb5ae972eb033e2ca6f4553aeb6f92dee186.nq.gz
    ├── 12db1b0bb2ad8523bc2420db39ee9502927ad778.nq.gz
    ├── 1303170d00dabfbf07e3339b32d9e19dffcb949b.nq.gz
    ├── 13314db788b536bea62c0b57e5c50a8e05ef713c.nq.gz
    ├── 133a6231a5b53fd2f073799ca1bd07c50abe40ae.nq.gz
    ├── 1356cd22fc9e11b0cd87a2585ebe48daf973f3c1.nq.gz
    ├── 136aa41c26338511eb0895146e3fa8259f4415b3.nq.gz
    ├── 13bb7f03ad049ca653c148ff9325412b96b8a7ba.nq.gz
    └── 13cd9336732a0854dae25b53b34e4b2e749b5897.nq.gz

7 directories, 200 files
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

[encode/httpx](https://github.com/encode/httpx)

---
*Parsed on 2026-03-27 by [repolex](https://repolex.ai)*
