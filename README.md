# Karlsruhe Institute of Technology (karlsruhe-institute-of-technology)

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
