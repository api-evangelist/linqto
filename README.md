# Linqto

Linqto is a San Jose, California private-markets investment platform that gives individual
accredited investors access to equity in mid-to-late-stage private technology companies before
an IPO or acquisition. Rather than acting as a marketplace intermediary, Linqto buys shares
itself and delivers them to investors as units in a series-LLC private fund ("Liquidshares")
holding the underlying company's stock, charging a single purchase premium with no carry,
profit, legal, or administrative fees. Investing runs through the web and mobile application at
app.linqto.com. The company filed for Chapter 11 protection in the U.S. Bankruptcy Court for
the Southern District of Texas in 2025 and has paused transactions while continuing operations.

- Website: https://www.linqto.com/
- Application: https://app.linqto.com/
- GitHub: https://github.com/Linqto-Team

## API surface

Linqto publishes **no public developer API, OpenAPI/Swagger specification, GraphQL endpoint,
MCP server, A2A agent card, SDK, or developer portal.** Contract discovery on 2026-08-01 probed
every candidate spec and `/.well-known/` path across `www.linqto.com`, `app.linqto.com`, and
`api.app.linqto.com`; `api.linqto.com`, `developer.linqto.com`, `docs.linqto.com`, and
`status.linqto.com` do not resolve. The investor application is served by a private,
session-authenticated backend at `api.app.linqto.com` that publishes no contract and is
deliberately not catalogued as an API surface.

The only anonymously callable machine-readable surfaces are the WordPress REST API
(`/wp-json/`, 472 routes) and the RSS feed behind the marketing site.

## Artifacts

| Path | What it records |
|---|---|
| `apis.yml` | Company identity, the two public surfaces, and link properties |
| `well-known/linqto-well-known.yml` | `/.well-known/` + full contract-discovery probe record |
| `packages/linqto-packages.yml` | Package-registry and GitHub-org search results (no SDK) |
| `security/linqto-domain-security.yml` | Probed TLS / HSTS / DNSSEC / CAA / SPF / DMARC posture |
| `llms/linqto-llms.txt` | Generated llms.txt for the provider |
