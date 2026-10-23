# AxisVela

**English** | [简体中文](README.zh-CN.md)

**Independent developer projects** for governed autonomous systems — agents,
workflows, robots, and digital twins — built in public.

AxisVela is a solo-maintainer collection, not a company. The public repositories
are the open surface: runnable frameworks, protocols, contracts, SDKs, and
reference implementations. Core and enterprise editions are developed privately
and offered separately.

## Full project map

For the complete map — every project, its goals, relationships, concepts, and
where to start — see [AxisVela Open](https://github.com/axisvela/axisvela-open)
or the [documentation site](https://axisvela.github.io/axisvela-open/).

## Start here

### [praxo-core](https://github.com/axisvela/praxo-core) — MIT agent framework

The main entry point to this ecosystem. A real, runnable Go framework — not a
contract shell:

- governed agent loop and model/tool/memory/event primitives
- plugins, sandboxing, and policy enforcement
- MCP, Anthropic, and OpenAI adapters
- OpenTelemetry instrumentation and benchmarks
- bilingual docs and an MkDocs site

Clone it first. You do not need anything else in this organization to run it.

```bash
git clone https://github.com/axisvela/praxo-core
cd praxo-core
go test ./...
```

## Ecosystem map

The public repos fall into three layers.

### Runnable frameworks and protocols

| Repository | What it is |
| --- | --- |
| [praxo-core](https://github.com/axisvela/praxo-core) | MIT agent framework: loop, adapters, sandbox, policy, OTel |
| [harmovela](https://github.com/axisvela/harmovela) | Open coordination protocol for autonomous systems |
| [TAXOVELA](https://github.com/axisvela/TAXOVELA) | AI-native enterprise architecture design and validation skills + CLI |
| [enterprise-autonomy](https://github.com/axisvela/enterprise-autonomy) | Introduction and end-to-end examples for the wider ecosystem |

### Open product surfaces

Each `*-open` repository publishes the Apache-2.0 integration surface of a
product: versioned contracts, SDKs, CLI, examples, and in some cases signed
binaries. The runtime behind it lives in a separate private core repo.

| Domain | Public surface |
| --- | --- |
| Development coordination | [coordivela-open](https://github.com/axisvela/coordivela-open) |
| Durable workflow | [rheovela-open](https://github.com/axisvela/rheovela-open) |
| Agent memory | [mnemovela-open](https://github.com/axisvela/mnemovela-open) |
| Identity and authorization | [aegivela-open](https://github.com/axisvela/aegivela-open), [eidovela-open](https://github.com/axisvela/eidovela-open), [NOMIVELA-open](https://github.com/axisvela/NOMIVELA-open) |
| Integration gateway | [limenora-open](https://github.com/axisvela/limenora-open) |
| Semantic and knowledge fabric | [gnosivela-open](https://github.com/axisvela/gnosivela-open), [ontovela-open](https://github.com/axisvela/ontovela-open) |
| Verification and simulation | [tekmovela-open](https://github.com/axisvela/tekmovela-open), [peiravela-open](https://github.com/axisvela/peiravela-open), [SYNDOVELA-open](https://github.com/axisvela/SYNDOVELA-open) |
| Capability and planning | [moduregis-open](https://github.com/axisvela/moduregis-open), [orchadyn-open](https://github.com/axisvela/orchadyn-open) |
| Operations and collaboration | [symbivela-open](https://github.com/axisvela/symbivela-open), [noetivela-open](https://github.com/axisvela/noetivela-open), [kinetovela-open](https://github.com/axisvela/kinetovela-open) |

### Adjacent projects

| Repository | What it is |
| --- | --- |
| [AXISRobo-PAMP](https://github.com/axisvela/AXISRobo-PAMP) | Practical platform for enterprise architecture management |

## How to engage

- **Trying the ecosystem:** start with [praxo-core](https://github.com/axisvela/praxo-core).
  If it does not run for you, that is a bug worth reporting.
- **Using an open surface:** open an issue on the specific `*-open` repository.
- **Commercial or enterprise use:** open an issue on the relevant repository and
  ask for the enterprise contact path.
- **Security reports:** follow the `SECURITY.md` in the affected repository rather
  than filing a public issue.

## Status

These projects are early stage. Public contracts are versioned, but APIs may
change between minor releases until a repository declares 1.0. Each repository's
`CHANGELOG.md`, `ROADMAP.md`, and release tags are the source of truth.
