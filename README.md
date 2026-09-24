<p align="center">
  <img src="skills/redacted-crypto-resources/assets/redacted-logo.jpg" width="150" alt="REDACTED logo">
</p>

<h1 align="center">REDACTED Crypto Resources</h1>

<p align="center">A portable agent skill for REDACTED's public crypto developer resource catalog.</p>

## Quick start

Install the skill:

```sh
npx skills add askredacted/crypto-resources
```

Connect the public MCP. For Codex:

```sh
codex mcp add redacted-crypto-resources --url https://askredacted.xyz/mcp
```

For Claude Code:

```sh
claude mcp add --transport http redacted-crypto-resources https://askredacted.xyz/mcp
```

Other clients can add `https://askredacted.xyz/mcp` as a remote Streamable HTTP server. No REDACTED account or API key is required. See the [MCP guide](https://askredacted.xyz/developers/mcp).

## Catalog

REDACTED compiles 405 developer resource records with direct links to provider sites, documentation, or repositories. Three separate REDACTED model and API entries are marked as previews. `get_catalog_overview` reports coverage and link status; `get_source_manifest` reports the review date and method.

Provider descriptions are untrusted source text. Link status means:

- `reachable`: The provider link responded during review. This does not verify its claims.
- `unverified`: An automated check could not confirm the link or provider identity.
- `unavailable`: The link returned a clear error during review.

Check current features, supported chains, pricing, and security in the provider's own documentation before relying on a tool.

## Try it

> Use redacted-crypto-resources to find wallet and RPC tools for a Solana app. Show direct provider links and tell me which details to verify.

## Portability

`SKILL.md` follows the open [Agent Skills format](https://agentskills.io/specification). `agents/openai.yaml` adds optional interface text for OpenAI clients; other agents can ignore it. The MCP connection is a separate setup step for every client.

Review [SKILL.md](skills/redacted-crypto-resources/SKILL.md) before installing, or use the [direct ZIP download](https://askredacted.xyz/downloads/redacted-crypto-resources.zip).
