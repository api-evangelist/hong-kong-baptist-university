# Hong Kong Baptist University (hong-kong-baptist-university)

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

Hong Kong Baptist University (HKBU) is a publicly funded research university in Hong Kong SAR, ranked #253 in the QS World University Rankings 2025. This repository catalogs HKBU's public, machine-readable developer/API footprint as an APIs.json provider profile. The most concrete public API is the HKBU Scholars Pure Web Service API (Elsevier Pure, OpenAPI 3), used for research-information metadata. A mobile-app backend host exists but is gated and undocumented for external developers.

- APIs.json: https://raw.githubusercontent.com/api-evangelist/hong-kong-baptist-university/refs/heads/main/apis.yml
- Run with Naftiko: https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=hong-kong-baptist-university-api-evangelist&utm_content=repo

## Type

- Index
- Consumer
- 3rd-Party

## Tags

Education, Higher Education, University, Research, Hong Kong, Pure, Research Information

## APIs

- **HKBU Scholars Pure Web Service API** — REST API powering the HKBU Scholars research portal (Elsevier Pure); exposes research outputs, persons, organisations, projects, and activities. Public OpenAPI 3.0.1 contract and RapiDoc docs are available; data endpoints require an API key.
  - Docs: https://scholars.hkbu.edu.hk/ws/api/rapidoc.html
  - OpenAPI: https://scholars.hkbu.edu.hk/ws/api/openapi.yaml
  - Base URL: https://scholars.hkbu.edu.hk/ws/api/
- **HKBU Mobile App Backend (gated)** — Backend host (mapp-api.hkbu.edu.hk) serving the official HKBU mobile app. No public developer documentation, OpenAPI spec, or self-service sign-up; listed for completeness only.
  - Reference: https://mapp-api.hkbu.edu.hk/html/app_privacy_policy.html

## Plans / Rate Limits / FinOps

- Plans & Pricing: [plans/hong-kong-baptist-university-plans-pricing.yml](plans/hong-kong-baptist-university-plans-pricing.yml)
- Rate Limits: [rate-limits/hong-kong-baptist-university-rate-limits.yml](rate-limits/hong-kong-baptist-university-rate-limits.yml)
- FinOps: [finops/hong-kong-baptist-university-finops.yml](finops/hong-kong-baptist-university-finops.yml)

## Timestamps

- Created: 2026-06-03
- Modified: 2026-06-03

## Common Properties

- Website: https://www.hkbu.edu.hk/
- GitHub: https://github.com/HKBUNLP (research-group org; no institution-wide org found)
- LinkedIn: https://hk.linkedin.com/school/hong-kong-baptist-university/
- Twitter/X: https://x.com/hkbaptistu
- Review: [review.yml](review.yml)

## Notes

- All endpoints were live-checked on 2026-06-03; no endpoints were fabricated.
- The Pure API OpenAPI contract and RapiDoc docs return HTTP 200; Pure data and OAI-PMH endpoints return HTTP 401 pending an API key/authorization, which is expected behavior.
- There is no central institutional developer portal and no organization-wide GitHub org; only research-group orgs (e.g., HKBUNLP, HKBU-HPML) publish code publicly.
- The OIRP Data Hub (data-hub.hkbu.edu.hk) returned 503, the digital scholarship portal (digital.lib.hkbu.edu.hk) returned 403 to an automated client, and the institutional repository host (repository.hkbu.edu.hk) did not resolve from this network at review time.

## Maintainers

- Kin Lane — kin@apievangelist.com
