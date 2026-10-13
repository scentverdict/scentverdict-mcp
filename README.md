<p align="center">
  <a href="https://scentverdict.com">
    <picture>
      <source media="(prefers-color-scheme: dark)" srcset="assets/scentverdict-lockup-dark.png">
      <img alt="ScentVerdict" src="assets/scentverdict-lockup-light.png" width="420">
    </picture>
  </a>
</p>

<p align="center">
  <strong>Fragrance verdicts, similarity scores, scent profiles and drydowns, with local prices.</strong><br>
  A free, hosted, read-only MCP server. No account, no sign-in, no API key.
</p>

<p align="center">
  <a href="https://scentverdict.com/connect">Connect guide</a> &middot;
  <a href="https://scentverdict.com">scentverdict.com</a> &middot;
  <code>https://scentverdict.com/mcp</code>
</p>

---

## ScentVerdict MCP server

ScentVerdict is a free, hosted MCP server. There is nothing to install and no account, sign-in or API key. All six tools are read-only.

- Endpoint: `https://scentverdict.com/mcp` (Streamable HTTP)
- Documentation: https://scentverdict.com/connect
- Website: https://scentverdict.com
- Official MCP registry name: `com.scentverdict/fragrances`
- Contact: hello@scentverdict.com

This repository holds only the listing metadata for directories that list a server from a public repository. The server itself is hosted at scentverdict.com and is not published here.

## Tools

| Tool | What it does |
|---|---|
| `get_fragrance` | Look up one fragrance: notes, verdict, concentration, launch year, and the lowest current bottle price for the user's country |
| `search_fragrances` | Resolve a partial or ambiguous name to the right catalogue entry |
| `find_similar_fragrances` | Find fragrances similar to one you know, optionally steered cheaper, fresher, longer lasting or less sweet |
| `recommend_fragrances` | Recommend by season, occasion, budget, strength and favourite notes |
| `compare_fragrances` | Compare two fragrances side by side |
| `get_scent_profile` | Show how a fragrance develops from opening to drydown |

Prices follow the `country` argument (an ISO code such as `GB` or `US`) and are in the shop's own currency.

## Add it

**Claude:** Customize, Connectors, Add custom connector, URL `https://scentverdict.com/mcp`, no authentication.

**ChatGPT:** add `https://scentverdict.com/mcp` as a custom connector with no authentication.

**Gemini CLI:** `gemini extensions install https://github.com/scentverdict/scentverdict-mcp`

**Any MCP client:** point it at `https://scentverdict.com/mcp` over Streamable HTTP.

## Try it

- What is Baccarat Rouge 540 and is it worth the money?
- Recommend a winter fragrance for the office, under 80 pounds.
- How does Dior Sauvage develop over the day?
- He wears Aventus. What else would he like?

## Operator

DBHQ Consulting Ltd, trading as ScentVerdict (UK company 06839674). Privacy: https://scentverdict.com/privacy. Terms: https://scentverdict.com/terms.

The version in `gemini-extension.json`, `lhm.plugin.json` and `package.json` follows the server version in the official registry.
