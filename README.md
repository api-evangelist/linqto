# Linqto

<!-- API-EVANGELIST-PROVENANCE:BEGIN -->
> ### About this repository
>
> **This is not our API.** This repository is an independent, third-party profile of a company's
> **publicly available** API surface, maintained by [API Evangelist](https://apievangelist.com).
> API Evangelist does not operate, host, resell, or support this company's APIs, and is not
> affiliated with or endorsed by the company unless stated on the profile.
>
> **Where the information came from.** Everything here is assembled from material a member of the
> public can reach with a browser and no credentials — the company's own website, developer portal
> and documentation, the specifications it publishes for public use (OpenAPI, AsyncAPI, JSON Schema,
> `apis.json`, `llms.txt` and similar), its public repositories, and its public status, pricing and
> changelog pages. **Nothing here is obtained by breaching a system, defeating an access control, or
> using credentials of any kind.**
>
> **The rating is an independent assessment.** The Kin Score and Agent Readiness rating are
> independently calculated scores of a company's *public* API artifacts, produced by API Evangelist
> against a published rubric. They are not certifications, endorsements, security assessments, or
> audits, and they score published artifacts — not the quality, safety, or security of the software.
>
> **Corrections, re-scores, and removal are free.** No partnership, contract, or purchase is
> required, and you do not need to justify the request.
>
> - **Something wrong?** Open an issue on this repository, or email
>   [info@apievangelist.com](mailto:info@apievangelist.com).
> - **Published something new?** Ask for a re-score and we will re-run the rating.
> - **Want the listing taken down?** Say so and we will honor it. The profile is reduced to your
>   company name, a factual description, and a link to your own site, and the company is recorded as
>   **unrated** — never scored zero for having asked.
>
> **Response times.** Acknowledgement within **one business day**; removal or restriction within
> **two business days**; corrections and re-scores within **five business days**.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

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
