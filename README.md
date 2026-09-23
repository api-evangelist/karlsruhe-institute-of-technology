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
> **Not from the company, and here with a question?** You are welcome here — we would rather be the
> front line and point you the right way than have a good report go nowhere. What this repository
> can answer is narrow, though, so it is worth knowing who you are actually looking for:
>
> - **A question about how the API works, an account, billing, or a bug in the service** — that is
>   the company's own support, not us. We profile this API; we do not operate it and cannot see
>   your account.
> - **A bug in an open-source project we only catalog** — file it on that project's own repository.
>   This has happened with a real and correct bug report that reached us instead of the people who
>   could fix it, which helped nobody.
> - **Anything about this listing itself** — the description, the tags, the rating, a missing or
>   wrong artifact — is ours. Open an issue here.
> - **Not sure, or something general about API Evangelist or APIs.io** — open an issue on the
>   [APIs.io Inbox](https://github.com/api-search/inbox) and we will route it.
>
> **This repository contains no software, and we will never ask you to download anything.** There is
> no build, release, installer, or binary here — only text and machine-readable API descriptions, so
> there is nothing here that can be "corrupt" or need "repairing". Any issue, comment, or email
> claiming otherwise and offering a download link is not from us and is hostile. Do not follow the
> link; it is a lure. Report it to GitHub and, if you like, tell us at
> [info@apievangelist.com](mailto:info@apievangelist.com) so we can take it down.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

Karlsruhe Institute of Technology (KIT) is a public research university and national research center of the Helmholtz Association in Karlsruhe, Germany, and a member of the TU9 alliance. This repository catalogs KIT's public programmable footprint as an [APIs.json](https://apisjson.org) provider profile, re-profiled on 2026-09-01 under the API Evangelist university pipeline, which settles **who operates each surface** before anything is saved.

KIT publishes **no central developer portal and no institution-authored API contract**. `api.kit.edu`, `developer.kit.edu`, `data.kit.edu` and `opendata.kit.edu` do not resolve. What KIT does operate — all probed live, not inferred from links — is a set of standards-protocol and self-hosted surfaces on its own `kit.edu` domain, plus two registry memberships. Three of those surfaces answer with a **product's** generic contract (Koha, RADAR, Open WebUI) rather than KIT's own engineering; the deployments are recorded here and those contracts are deliberately **not** saved under KIT's name.

- APIs.json: https://raw.githubusercontent.com/api-evangelist/karlsruhe-institute-of-technology/refs/heads/main/apis.yml
- Run it with Naftiko: https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=karlsruhe-institute-of-technology-api-evangelist&utm_content=repo

## Type

- University / Technical University / Index / Consumer / 3rd-Party

## Tags

Education, Higher Education, University, Technical University, Germany, Europe, Research, Research Data, Open Access, Open Science, Institutional Repository, Library, OAI-PMH, Identity Federation, Shibboleth, Research Computing, TU9, Helmholtz Association

## Surfaces, by operator

| Surface | `x-operator` | Contract saved? |
|---|---|---|
| **KITopen OAI-PMH Interface** — OAI-PMH 2.0 on the KIT Library's own dbkit framework. `verb=Identify` returns `repositoryName "KITopen"`. Base: https://dbkit.bibliothek.kit.edu/oai/ | `institution` | protocol, no OpenAPI |
| **KIT Library Catalogue REST API** — self-hosted Koha at https://katalog.bibliothek.kit.edu/api/v1/, 242 paths, 16 keyless `/public` paths returning KIT's own branch records | `institution` (deployment) | **No** — `info.contact` is the Koha Development Team |
| **RADAR4KIT** — research-data repository, a tenancy on FIZ Karlsruhe's RADAR service running on KIT SCC infrastructure. Backend https://radar.kit.edu/radar-backend/ answers 401 | `tenant` | **No** — the RADAR Archive API is FIZ Karlsruhe's |
| **KIT Shibboleth Identity Provider** — SAML 2.0 metadata at https://idp.scc.kit.edu/idp/shibboleth, registered in DFN-AAI since 2010, bwIDM entity category | `federation` | **No** — the federation's contract is DFN's |
| **KIT OpenID Connect Provider** — Keycloak realm `kit` at https://oidc.scc.kit.edu/auth/realms/kit, eleven grant types | `institution` | **No** — Keycloak's admin contract is the product's |
| **KI-Toolbox** — KIT's generative-AI service (Open WebUI 0.10.2) serving SCC-hosted LLMs behind the KIT Account. 458-path OpenAPI 3.1.0 at `/openapi.json` | `institution` (deployment) | **No** — `info.title` is "Open WebUI", no `servers[]` |
| **DataCite membership** — direct member `kit`, ROR `04t3en479`, client `TIB.KIT4RADAR` | `registry` | never |
| **Crossref membership** — member 37766, KIT Library, prefix 10.58895, 456 DOIs | `registry` | never |
| **ROR record** — https://ror.org/04t3en479 | `registry` | never |

## Conformance

`education` regime standards confirmed against live endpoints or contract declarations, in [conformance/karlsruhe-institute-of-technology-conformance.yml](conformance/karlsruhe-institute-of-technology-conformance.yml):

- **oai-pmh** — KITopen `verb=Identify`, `ListMetadataFormats` (oai_dc, epicur, oai_datacite), `ListSets`
- **saml** — SAML 2.0 IdP metadata, 4 SSO bindings
- **shibboleth** — Shibboleth IdP paths + DFN-AAI `registrationAuthority`
- **datacite** — direct member, plus the `oai_datacite` prefix served by KIT's own OAI endpoint
- **crossref** — KIT Library Crossref member, prefix 10.58895

Not evidenced and deliberately not claimed: `orcid` (prose only, no contract declaration), `lti`, `scim`, `oneroster`, `ed-fi`, `caliper`, `qti`.

## Plans / Rate Limits / FinOps

- Plans: [plans/karlsruhe-institute-of-technology-plans-pricing.yml](plans/karlsruhe-institute-of-technology-plans-pricing.yml)
- Rate Limits: [rate-limits/karlsruhe-institute-of-technology-rate-limits.yml](rate-limits/karlsruhe-institute-of-technology-rate-limits.yml)
- FinOps: [finops/karlsruhe-institute-of-technology-finops.yml](finops/karlsruhe-institute-of-technology-finops.yml)

## Timestamps

- Created: 2026-06-03
- Modified: 2026-09-01

## Common Properties

- Website: https://www.kit.edu/english/
- Research Repository: https://publikationen.bibliothek.kit.edu/ and https://radar.kit.edu/
- Library Catalog: https://katalog.bibliothek.kit.edu/
- Course Catalog: https://campus.studium.kit.edu/ (CAS Campus, vendor product, no public API)
- Identity Federation: https://idp.scc.kit.edu/idp/shibboleth
- Research Computing: https://www.nhr.kit.edu/ (NHR@KIT / HoreKa)
- AI Policy: https://www.kit.edu/downloads/KI-Leitlinien-de.pdf
- AI Tooling: https://www.scc.kit.edu/en/services/ki-toolbox.php
- GitHub Organization: https://github.com/KIT-SCC (KIT code is spread across many institute-level orgs)
- Source Code: https://gitlab.kit.edu/ (self-hosted GitLab; its API v4 answers keyless, but the contract is GitLab's)
- security.txt: https://www.kit.edu/.well-known/security.txt (PGP-signed, `cert@kit.edu`)
- Review: [review.yml](review.yml)

## Notes on this re-profile

Every surface above was probed with live HTTP on 2026-09-01; no endpoints were fabricated and no vendor contract was saved under KIT's name. Changes from the 2026-06-03 profile:

1. The standalone **"dbkit API"** entry was **removed**. It carried no `baseURL` and no documented endpoint; https://www.bibliothek.kit.edu/english/dbkit.php names an "API interface" but publishes no base URL, parameters or formats. dbkit's one evidenced public interface is the KITopen OAI-PMH endpoint, which is recorded as its own entry.
2. The RADAR documentation pointer `https://www.bibliothek.kit.edu/english/radar.php` was **dead** (302 into the library's soft-404 search page) and was replaced with https://www.bibliothek.kit.edu/english/radar4kit.php.
3. Five surfaces were **added**: the self-hosted Koha catalogue API, the Keycloak OIDC realm, the KI-Toolbox, the Crossref membership and the ROR record; the DataCite membership was promoted from prose to an evidenced `registry` entry.
4. Every `apis[]` entry now carries an `x-operator`, and the `Open Data` tag was replaced with `Open Access` / `Open Science` — KIT publishes CC0 bibliographic metadata via OAI-PMH but operates no open data portal.

The LinkedIn page returns HTTP 999 (LinkedIn bot-block) but exists.

## Maintainers

- Kin Lane — kin@apievangelist.com
