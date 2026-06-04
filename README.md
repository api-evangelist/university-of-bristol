# University of Bristol (university-of-bristol)

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
