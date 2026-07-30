# Kite

Kite (gokite.ai, formerly Zettablock) builds agentic payment infrastructure for the machine-to-machine
economy. Kite Agent Passport gives autonomous AI agents their own identity, a funded wallet, user-set
spending rules, delegated payment authority, and verifiable on-chain receipts — driven from a coding
agent through the `kpass` and `ksearch` CLIs and a bundle of published Passport agent skills.

Kite also operates Kite Chain, an EVM-compatible Avalanche-subnet Layer 1 (mainnet chain ID 2366,
testnet 2368), a stablecoin gasless transfer relayer built on EIP-3009 signed authorizations, and an
x402 HTTP-402 payment surface with support for the Stripe/Tempo Machine Payments Protocol (MPP).

Backed by: general-catalyst (also PayPal Ventures — $18M Series A, September 2025)

## APIs

| API | Base URL |
| --- | --- |
| Kite Chain JSON-RPC (Mainnet) | https://rpc.gokite.ai/ |
| Kite Chain JSON-RPC (Testnet) | https://rpc-testnet.gokite.ai/ |
| Kite Stablecoin Gasless Transfer API | https://gasless.gokite.ai |

## Artifacts

`llms/` `mcp/` `cli/` `packages/` `skills/` `changelog/` `lifecycle/` `conventions/`
`authentication/` `errors/` `conformance/` `sandbox/` `well-known/` `security/`

## Notes

Kite publishes **no OpenAPI** — its API Reference page is an explicit "Coming soon" placeholder — so
no `openapi/`, `overlays/`, `scopes/`, `data-model/`, or generated agent-skill markdown are present.
Its agent-facing discovery runs through `llms.txt` (with per-collection shards and an MCP endpoint)
rather than `/.well-known/`, all of which returned 404.
