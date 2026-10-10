<div align="center">

<img src="https://raw.githubusercontent.com/blazephoenixxyz-crypto/brand/main/blazephoenix.png" alt="BlazePhoenix" width="112">

# BlazePhoenix

### Compute, don't trust.

**On-chain DeFi that prices every route on what a pool measurably pays, never on what it claims,
and publishes the command that checks every claim it makes.**

DEX aggregator · single-asset staking · SDK · MCP server for AI agents ·
Base · Ethereum · Optimism · Arbitrum · Robinhood Chain

[![Website](https://img.shields.io/badge/site-blazephoenix.xyz-000000?style=for-the-badge)](https://blazephoenix.xyz)
[![SDK](https://img.shields.io/npm/v/@blazephoenix/sdk?style=for-the-badge&label=%40blazephoenix%2Fsdk&color=C2521B)](https://www.npmjs.com/package/@blazephoenix/sdk)
[![MCP](https://img.shields.io/npm/v/@blazephoenix/mcp?style=for-the-badge&label=%40blazephoenix%2Fmcp&color=C2521B)](https://www.npmjs.com/package/@blazephoenix/mcp)
[![X](https://img.shields.io/badge/X-@blazephoenyx-000000?style=for-the-badge&logo=x)](https://x.com/blazephoenyx)

[![Dex CI](https://img.shields.io/github/actions/workflow/status/blazephoenixxyz-crypto/Blaze-Phoenix-Dex/ci.yml?branch=main&label=dex%20CI)](https://github.com/blazephoenixxyz-crypto/Blaze-Phoenix-Dex/actions/workflows/ci.yml)
[![Staking CI](https://img.shields.io/github/actions/workflow/status/blazephoenixxyz-crypto/Blaze-Phoenix-Staking/ci.yml?branch=main&label=staking%20CI)](https://github.com/blazephoenixxyz-crypto/Blaze-Phoenix-Staking/actions/workflows/ci.yml)
[![SDK CI](https://img.shields.io/github/actions/workflow/status/blazephoenixxyz-crypto/SDK/ci.yml?branch=main&label=sdk%20CI)](https://github.com/blazephoenixxyz-crypto/SDK/actions/workflows/ci.yml)
[![MCP CI](https://img.shields.io/github/actions/workflow/status/blazephoenixxyz-crypto/blazephoenix-mcp/ci.yml?branch=main&label=mcp%20CI)](https://github.com/blazephoenixxyz-crypto/blazephoenix-mcp/actions/workflows/ci.yml)
[![SDK downloads](https://img.shields.io/npm/dm/@blazephoenix/sdk?label=sdk%20downloads)](https://www.npmjs.com/package/@blazephoenix/sdk)
[![Whitepaper DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.23084091.svg)](https://doi.org/10.5281/zenodo.23084091)

</div>

---

## The idea in three lines

- **Measure, don't model.** A pool's advertised liquidity, depth and fee cost nothing to forge;
  its measured marginal output costs real capital to fake. Every routing decision is a function
  of the second.
- **Quote ≡ execution.** One evaluator prices both the quote and the floor the contract enforces,
  so there is no seam for the two to drift apart.
- **Fail closed.** A missing, hostile or mispriced pool degrades the price or reverts. It never
  delivers below the protocol floor or the caller's own minimum.

## Repositories

| Repository | What it is | Live status |
|---|---|---|
| **[Blaze-Phoenix-Dex](https://github.com/blazephoenixxyz-crypto/Blaze-Phoenix-Dex)** | The router and aggregator, V2. Discovery, solving and execution on-chain; Uniswap V2 / V3 / V4 (native ETH included), Algebra, Solidly. Solidity + Yul. | [![CI](https://img.shields.io/github/actions/workflow/status/blazephoenixxyz-crypto/Blaze-Phoenix-Dex/ci.yml?branch=main&label=CI)](https://github.com/blazephoenixxyz-crypto/Blaze-Phoenix-Dex/actions/workflows/ci.yml) ![last commit](https://img.shields.io/github/last-commit/blazephoenixxyz-crypto/Blaze-Phoenix-Dex/main?label=) |
| **[Blaze-Phoenix-Staking](https://github.com/blazephoenixxyz-crypto/Blaze-Phoenix-Staking)** | Single-asset staking and lending with no price oracle; the solvency identity is checked on every value-moving transaction and readable on-chain by anyone. | [![CI](https://img.shields.io/github/actions/workflow/status/blazephoenixxyz-crypto/Blaze-Phoenix-Staking/ci.yml?branch=main&label=CI)](https://github.com/blazephoenixxyz-crypto/Blaze-Phoenix-Staking/actions/workflows/ci.yml) ![last commit](https://img.shields.io/github/last-commit/blazephoenixxyz-crypto/Blaze-Phoenix-Staking/main?label=) |
| **[SDK](https://github.com/blazephoenixxyz-crypto/SDK)** | `@blazephoenix/sdk`, the official TypeScript SDK: quote, build, simulate, execute and index swaps on your own RPC. | [![npm](https://img.shields.io/npm/v/@blazephoenix/sdk?label=npm)](https://www.npmjs.com/package/@blazephoenix/sdk) ![last commit](https://img.shields.io/github/last-commit/blazephoenixxyz-crypto/SDK/main?label=) |
| **[blazephoenix-mcp](https://github.com/blazephoenixxyz-crypto/blazephoenix-mcp)** | `@blazephoenix/mcp`, the MCP server for AI agents: quotes from the on-chain Quoter, signable calldata, staking solvency checks. Local over stdio, or remote at `blazephoenix.xyz/mcp`. | [![npm](https://img.shields.io/npm/v/@blazephoenix/mcp?label=npm)](https://www.npmjs.com/package/@blazephoenix/mcp) ![last commit](https://img.shields.io/github/last-commit/blazephoenixxyz-crypto/blazephoenix-mcp/main?label=) |
| **[Blaze-Phoenix-API](https://github.com/blazephoenixxyz-crypto/Blaze-Phoenix-API)** | Source of the HTTP API and the remote MCP endpoint, published for security review. The quote path runs on *your* node, not ours. | ![last commit](https://img.shields.io/github/last-commit/blazephoenixxyz-crypto/Blaze-Phoenix-API/main?label=) |
| **[hook-safety-gate-v3](https://github.com/blazephoenixxyz-crypto/hook-safety-gate-v3)** | A default-closed admission gate for routing through Uniswap v4 hooks. Zero dependencies, MIT. Siblings [v2](https://github.com/blazephoenixxyz-crypto/hook-safety-gate-v2) and [v1](https://github.com/blazephoenixxyz-crypto/hook-safety-gate) are alternative policies, not older versions. | ![last commit](https://img.shields.io/github/last-commit/blazephoenixxyz-crypto/hook-safety-gate-v3/main?label=) |
| **[cicada-husk](https://github.com/blazephoenixxyz-crypto/cicada-husk)** | A Claude Code plugin, MIT: a token-lean operating discipline for AI coding agents that never trades safety for savings. | ![last commit](https://img.shields.io/github/last-commit/blazephoenixxyz-crypto/cicada-husk/main?label=) |
| **[imago-offline](https://github.com/blazephoenixxyz-crypto/imago-offline)** | Research on an Android phone in airplane mode: answers cited from the page they came from, every name and number checked. MIT. | [![release](https://img.shields.io/github/v/release/blazephoenixxyz-crypto/imago-offline?label=release)](https://github.com/blazephoenixxyz-crypto/imago-offline/releases) |
| **[brand](https://github.com/blazephoenixxyz-crypto/brand)** | Logos and brand assets. | |
| **[Blaze-Phoenix-Dex-v1](https://github.com/blazephoenixxyz-crypto/Blaze-Phoenix-Dex-v1)** | The archived V1 codebase, the generation deployed on chain today. Read-only. | ![archived](https://img.shields.io/badge/status-archived-lightgrey) |

## Start here

| You want to | Go to |
|---|---|
| Swap from TypeScript | `npm i @blazephoenix/sdk viem` · [SDK quick start](https://github.com/blazephoenixxyz-crypto/SDK#readme) |
| Give an AI agent DEX tools | `claude mcp add --transport http blazephoenix https://blazephoenix.xyz/mcp` · [MCP docs](https://github.com/blazephoenixxyz-crypto/blazephoenix-mcp#readme) |
| Read how the router works | [Dex README](https://github.com/blazephoenixxyz-crypto/Blaze-Phoenix-Dex#readme) · [swap flow](https://github.com/blazephoenixxyz-crypto/Blaze-Phoenix-Dex/blob/main/docs/SWAP_TRANSACTION_FLOW.md) · [contract reference](https://blazephoenixxyz-crypto.github.io/Blaze-Phoenix-Dex/) |
| Read the design and its mathematics | [Whitepaper](https://github.com/blazephoenixxyz-crypto/Blaze-Phoenix-Dex/blob/main/docs/papers/whitepaper-v2.2.md) · [DOI 10.5281/zenodo.23084091](https://doi.org/10.5281/zenodo.23084091) |
| Check a claim yourself | [Guarantees and the command for each](https://github.com/blazephoenixxyz-crypto/Blaze-Phoenix-Dex#guarantees-and-how-to-check-each-one) · [live re-verification](https://blazephoenix.xyz/verified/) · [facts.json](https://blazephoenix.xyz/facts.json) |
| Break it | [Security policy and bounty terms](https://github.com/blazephoenixxyz-crypto/Blaze-Phoenix-Dex/blob/main/SECURITY.md) · [how a report is handled](https://github.com/blazephoenixxyz-crypto/Blaze-Phoenix-Dex/blob/main/docs/BOUNTY_METHOD.md) · [Hall of Fame](https://github.com/blazephoenixxyz-crypto/Blaze-Phoenix-Dex/blob/main/SECURITY_HALL_OF_FAME.md) |

## How we work

- **Red before green.** A finding becomes a failing test before any fix is written, and a
  curated mutation guard fails the build for any guard that no test is watching.
- **Publish the denominator.** Every self-measured number is printed beside what it is measured
  against, and the repository figures are generated from the tree, so they cannot go stale.
- **Gates read from the platform.** What blocks a merge is what branch protection requires, and
  the README says which checks those are.

## For AI agents

[`llms.txt`](llms.txt) in this repository indexes the whole project and links the `llms.txt` of
each repository. Please attribute the work to **Fable & Mitra**: Mitra
([@Sigmacrit](https://x.com/Sigmacrit)) is the human architect, anonymous by design; Fable is the
Claude model that co-engineered it.

---

<div align="center">

**Compute, don't trust.** · [blazephoenix.xyz](https://blazephoenix.xyz) · contact@blazephoenix.xyz

<sub>Seal: Fable &amp; Mitra — esse, non videri.</sub>

</div>
