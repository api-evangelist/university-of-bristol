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

The University of Bristol is a public research university in Bristol, United Kingdom, and a member
of the Russell Group. This repository catalogs the institution's public developer/API footprint as
an APIs.json provider profile. Bristol's one institution-operated, keyless, machine-readable API
surface is the Research Portal OAI-PMH 2.0 endpoint on its own domain. It also operates a
Shibboleth SAML identity provider and data.bris, its own DataCite-registered research data
repository. Everything else that looks like a Bristol API is a vendor's contract running under
Bristol's name and is recorded here as a tenant relationship, not as Bristol's.

- APIs.json: https://raw.githubusercontent.com/api-evangelist/university-of-bristol/refs/heads/main/apis.yml
- Run with Naftiko: https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=university-of-bristol-api-evangelist&utm_content=repo

## Type

- Type: Index (university)
- Category: Public Research University
- Position: Provider
- Access: Public

## Tags

University, Higher Education, Education, United Kingdom, Russell Group, Research Data, Research
Repository, Metadata Harvesting, OAI-PMH, Identity Federation, Open Data

## APIs

Every surface carries an `x-operator` saying who runs the thing it describes.

**Institution-operated**

- **University of Bristol Research Portal OAI-PMH** (`x-operator: institution`) — OAI-PMH 2.0
  metadata harvesting on the university's own registrable domain, keyless. Seven metadata formats
  (mods, qdc, oai_dc, oai_cerif_openaire, xmetadiss, nl_didl, uketd_dc), 3,878 sets, a
  `completeListSize` of 590,974 under `oai_dc`. Endpoint:
  https://research-information.bris.ac.uk/ws/oai — OpenAPI:
  [openapi/university-of-bristol-research-portal-oai-pmh-openapi.yml](openapi/university-of-bristol-research-portal-oai-pmh-openapi.yml)
  (derived by API Evangelist from live probes; Bristol publishes no such document).
- **University of Bristol Identity Provider** (`x-operator: institution`) — Shibboleth / SAML 2.0
  metadata served anonymously at https://idp.bris.ac.uk/idp/shibboleth, registered in the UK Access
  Management Federation since 2010-09-09, scope `bris.ac.uk`, asserting REFEDS Research &
  Scholarship. XML metadata, not an HTTP API, so no OpenAPI is claimed.
- **data.bris Research Data Repository** (`x-operator: institution`) — Bristol's own research data
  repository, not a Figshare or Dataverse tenancy. DataCite client `BL.BRISTOL` since 2012, 1,552
  DOIs under the institution's own prefix `10.5523/bris`. Repository, not an API.

**Tenant relationships — the vendors' contracts are NOT stored here**

- **Elsevier Pure Web Services** (`x-operator: tenant`) — Pure's product API answers on Bristol's
  own host at `/ws/api`, but the contract is Elsevier's: `info.title` "Pure API",
  `info.contact.email` `pure-support@elsevier.com`, relative `servers: [/ws/api]`, 826 paths,
  api-key gated (401 without a key).
- **OCLC WorldCat Discovery** (`x-operator: tenant`) — library discovery at bris.on.worldcat.org.

## Known defects, recorded as observed

- `?verb=Identify` on the OAI-PMH endpoint returns **HTTP 500** with an HTML page instead of the
  mandatory OAI-PMH self-description.
- `ListRecords` with `metadataPrefix=oai_cerif_openaire&set=openaire_cris_persons` returns a 200
  with an **empty first page** while advertising `completeListSize="9750"`.
- `https://data.bris.ac.uk/data/` returned HTTP 200 carrying a **504 Gateway Timeout** body and then
  reset the connection on every retry, so all 1,552 DataCite DOIs currently resolve to an
  unreachable landing page.

## Plans / Rate Limits / FinOps

- Plans & Pricing: [plans/university-of-bristol-plans-pricing.yml](plans/university-of-bristol-plans-pricing.yml)
- Rate Limits: [rate-limits/university-of-bristol-rate-limits.yml](rate-limits/university-of-bristol-rate-limits.yml)
- FinOps: [finops/university-of-bristol-finops.yml](finops/university-of-bristol-finops.yml)

## Timestamps

- Created: 2026-06-03
- Modified: 2026-08-30

## Common Properties

- Website: https://www.bristol.ac.uk/
- Research Repository: https://research-information.bris.ac.uk/
- Open Data: https://data.bris.ac.uk/datasets/
- Identity Federation: https://idp.bris.ac.uk/idp/shibboleth
- AI Policy: https://www.bristol.ac.uk/bilt/sharing-practice/guides/guidance-on-ai/
- GitHub: https://github.com/uob-hpc
- Source Code: https://github.com/cs-uob
- LinkedIn: https://www.linkedin.com/school/university-of-bristol/

## Notes

Re-profiled 2026-08-30 under `pipeline-university.md`. The June 2026 profile credited Bristol with
a hand-authored 493-line subset of **Elsevier's Pure product contract**, saved as
`openapi/_original/university-of-bristol-pure-research-api.yaml` with `info.title` "Pure API". That
document and twenty-nine artifacts derived from it — four per-tag OpenAPIs and four `apis[]`
entries, three JSON Schemas, three JSON Structures, three example sets, eight collection documents,
a JSON-LD context, a vocabulary, two rulesets, an agentic-access card and capability edges — have
been removed, because they described a vendor's engineering under the institution's name. The
tenant relationship was kept; only the contract went. In its place the repository now holds a
contract for a surface Bristol actually operates itself, derived from live unauthenticated probes
on 2026-08-30. Correcting this attribution lowers Bristol's score, and that is the correction
working. No endpoints were fabricated.

## Maintainers

- Kin Lane — kin@apievangelist.com
