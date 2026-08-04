# Karlsruhe Institute of Technology (karlsruhe-institute-of-technology)

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

Karlsruhe Institute of Technology (KIT) is a public research university and national research center in Karlsruhe, Germany, ranked #102 in the QS World University Rankings 2025. This repository catalogs KIT's public developer/API footprint as an [APIs.json](https://apisjson.org) provider profile. KIT's API presence is centered on research infrastructure run by the KIT Library and partner FIZ Karlsruhe — the KITopen institutional repository (dbkit framework, OAI-PMH) and the RADAR / RADAR4KIT research-data repository (REST, OAuth) — plus a Shibboleth identity provider operated by the Scientific Computing Center (SCC).

- APIs.json: https://raw.githubusercontent.com/api-evangelist/karlsruhe-institute-of-technology/refs/heads/main/apis.yml
- Run it with Naftiko: https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=karlsruhe-institute-of-technology-api-evangelist&utm_content=repo

## Type

- Index / Consumer / 3rd-Party

## Tags

Education, Higher Education, University, Research, Open Data, Research Data, Library, Germany

## APIs

- **KITopen OAI-PMH Interface** — central open-access institutional repository, OAI-PMH 2.0 harvesting. Docs: https://www.bibliothek.kit.edu/english/kitopen.php | Base: https://dbkit.bibliothek.kit.edu/oai/
- **dbkit API** — KIT Library web application framework providing API + OAI interfaces and bibliographic import/export (BibTeX, EndNote, RIS, CSL-JSON, ISI). Docs: https://www.bibliothek.kit.edu/english/dbkit.php
- **RADAR / RADAR4KIT Archive API** — research-data repository REST API (OAuth 2.0) for datasets, DOI assignment, and WebDAV upload; based on the RADAR service from FIZ Karlsruhe. Docs: https://radar.products.fiz-karlsruhe.de/en/radarfeatures/radar-api
- **KIT Shibboleth Identity Provider (SCC)** — Shibboleth/SAML 2.0 SSO and federated authentication. Endpoint: https://idp.scc.kit.edu/idp/shibboleth

## Plans / Rate Limits / FinOps

- Plans: [plans/karlsruhe-institute-of-technology-plans-pricing.yml](plans/karlsruhe-institute-of-technology-plans-pricing.yml)
- Rate Limits: [rate-limits/karlsruhe-institute-of-technology-rate-limits.yml](rate-limits/karlsruhe-institute-of-technology-rate-limits.yml)
- FinOps: [finops/karlsruhe-institute-of-technology-finops.yml](finops/karlsruhe-institute-of-technology-finops.yml)

## Timestamps

- Created: 2026-06-03
- Modified: 2026-06-03

## Common Properties

- Website: https://www.kit.edu/english/
- GitHub: https://github.com/KIT-SCC (Scientific Computing Center; KIT code is spread across many institute-level orgs)
- LinkedIn: https://www.linkedin.com/school/kit/
- Review: [review.yml](review.yml)

## Notes

All listed resources were confirmed via live HTTP probe or official documentation as of 2026-06-03; no endpoints were fabricated. KIT does not publish a single consolidated developer portal. The RADAR Archive API is gated — access requires an OAuth client ID and a dedicated API user activated by RADAR (Shibboleth accounts are not accepted for API access); the bare production base path returns 404 to unauthenticated requests. The LinkedIn page returns HTTP 999 (LinkedIn bot-block) but exists. KIT's open-source code is distributed across numerous institute GitHub organizations (KIT-SCC, KIT-MRT, KIT-IAI, KIT-ISAS, kit-algo, teco-kit, and others) rather than one official org.

## Maintainers

- Kin Lane — kin@apievangelist.com
