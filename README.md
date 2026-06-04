# Hong Kong Baptist University (hong-kong-baptist-university)

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
