# University of Bristol (university-of-bristol)

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

The University of Bristol is a public research university in Bristol, United Kingdom, ranked #58 in the QS World University Rankings 2025. This repository catalogs the institution's public developer/API footprint as an APIs.json provider profile. Bristol's strongest verifiable public API surface is research-oriented — the Bristol Research Portal (Elsevier Pure) with a documented REST API and OAI-PMH endpoint, plus the data.bris open research data repository.

- APIs.json: https://raw.githubusercontent.com/api-evangelist/university-of-bristol/refs/heads/main/apis.yml
- Run with Naftiko: https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=university-of-bristol-api-evangelist&utm_content=repo

## Type

- Type: Index
- Position: Consumer
- Access: 3rd-Party

## Tags

Education, Higher Education, University, Research, Open Data, United Kingdom

## APIs

- **Bristol Research Portal (Pure) API** — REST web services API for the Pure-powered research portal, documented with an OpenAPI 3.0.1 spec. Docs: https://research-information.bris.ac.uk/ws/api/524/api-docs/index.html | OpenAPI: https://research-information.bris.ac.uk/ws/api/openapi.json
- **Bristol Research Portal OAI-PMH** — OAI-PMH 2.0 metadata harvesting interface for the "University of Bristol Open Access Interface Repository". Endpoint: https://research-information.bris.ac.uk/ws/oai
- **data.bris Research Data Repository** — Open research data repository with DataCite DOIs. Docs: https://data.bris.ac.uk/data/about (no standard machine API path confirmed live)

## Plans / Rate Limits / FinOps

- Plans & Pricing: [plans/university-of-bristol-plans-pricing.yml](plans/university-of-bristol-plans-pricing.yml)
- Rate Limits: [rate-limits/university-of-bristol-rate-limits.yml](rate-limits/university-of-bristol-rate-limits.yml)
- FinOps: [finops/university-of-bristol-finops.yml](finops/university-of-bristol-finops.yml)

## Timestamps

- Created: 2026-06-03
- Modified: 2026-06-03

## Common Properties

- Website: https://www.bristol.ac.uk/
- Developer Portal: https://research-information.bris.ac.uk/
- GitHub: https://github.com/uob-hpc
- Source Code: https://github.com/cs-uob
- LinkedIn: https://www.linkedin.com/school/university-of-bristol/

## Notes

All catalogued API endpoints were probed live during review. The Pure REST API, its OpenAPI 3.0.1 spec, and the OAI-PMH 2.0 endpoint each returned HTTP 200. data.bris is a confirmed open data repository, but its standard CKAN API path (`/api/3/action/package_list`) returned 404, so no machine API endpoint was catalogued for it. The university operates no single unified institutional developer portal; the GitHub organizations listed are department-level (HPC, Computer Science) and publish open-source code rather than institutional APIs. No public status page resolved. No endpoints were fabricated.

## Maintainers

- Kin Lane — kin@apievangelist.com
