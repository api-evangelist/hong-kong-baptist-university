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

Hong Kong Baptist University (HKBU) is a publicly funded, UGC-supported research university in Hong Kong SAR. This repository catalogs HKBU's institution-operated, machine-readable footprint as an APIs.json provider profile. It was re-profiled on 2026-08-30 under the API Evangelist **university pipeline**, which settles *who operates* a surface before crediting any contract to the institution.

- APIs.json: https://raw.githubusercontent.com/api-evangelist/hong-kong-baptist-university/refs/heads/main/apis.yml
- Run with Naftiko: https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=hong-kong-baptist-university-api-evangelist&utm_content=repo

## Type

- Index / university
- Public Research University
- Consumer, Internal

## Tags

University, Higher Education, Education, Hong Kong, UGC-Funded, Identity Federation, Shibboleth, SAML, eduGAIN, Learning Management, LTI, Artificial Intelligence, Research Information, Elsevier Pure

## What changed on 2026-08-30

The 33 OpenAPI documents this repository previously held were **Elsevier's**, not HKBU's. Every one was titled `Pure activity … API`, version `5.35.0`, with `info.contact: pure-support@elsevier.com` — the same contract other Elsevier Pure institutions ship. They read as institution-owned only because they are served from `scholars.hkbu.edu.hk`, which DNS shows is a **CNAME to `hkbu.elsevierpure.com`** (`repository.hkbu.edu.hk` is aliased onto the same target).

All 33, the pristine `_original`, and 81 further files derived from them were removed — **115 files**: 64 collections, 3 JSON Schemas, 3 JSON Structures, 2 examples, a JSON-LD context, a vocabulary, two Spectral rulesets, an agentic-access map, an authentication summary, a capability-edge map, and two refine reports. The records and DOIs are HKBU's; the contract is Elsevier's, and it scores in Elsevier's repository. **Do not re-add them.**

## APIs

Every entry carries an `x-operator`.

**Institution-operated (4)**

- **HKBU Identity Federation — Shibboleth IdP / SAML 2.0 metadata** (`x-operator: institution`) — entityID `https://buidp01.hkbu.edu.hk/idp/shibboleth`, registered in eduGAIN by the Hong Kong Access Federation since 2018-03-14, scope `hkbu.edu.hk`. Metadata served anonymously: HTTP 200, `application/xml`, 12,306 bytes, declaring an IDPSSODescriptor and an AttributeAuthorityDescriptor across nine SAML 2.0 / SAML 1.1 / Shibboleth 1.0 endpoints plus SingleLogout. The one machine-readable interface HKBU both authors and operates end to end.
  - Metadata: https://buidp01.hkbu.edu.hk/idp/shibboleth
- **HKBU GenAI Platform API (undocumented, key-gated)** (`x-operator: institution`) — an Azure-OpenAI-shaped gateway at `genai.hkbu.edu.hk/general/rest/deployments/{deployment}/chat/completions` and `/embeddings`, routed internally to `/api/v0/rest/*`. Unauthenticated POST returns 401 `{"message":"API key is missing or invalid."}`; a POST carrying an `api-key` header returns a distinct key-validation 401, identifying the credential channel. No OpenAPI and no public developer docs are published.
  - Platform: https://genai.hkbu.edu.hk/
- **HKBU Moodle — IMS LTI 1.3 platform + web services** (`x-operator: institution`) — self-hosted Moodle at `buelearning.hkbu.edu.hk` publishing a live LTI 1.3 JWKS at `/mod/lti/certs.php` (HTTP 200, one RSA RS256 key) and an OAuth2 client-credentials token endpoint at `/mod/lti/token.php`. Moodle Web Services is enabled and token-gated. The software is Moodle's and the interface shape is IMS Global's — no contract is credited to HKBU — but the deployment, domain and signing keys are HKBU's.
  - JWKS: https://buelearning.hkbu.edu.hk/mod/lti/certs.php
- **HKBU Mobile App Backend (gated)** (`x-operator: institution`) — `mapp-api.hkbu.edu.hk`, first-party mobile client only. No public docs, no OpenAPI, no signup.
  - Reference: https://mapp-api.hkbu.edu.hk/html/app_privacy_policy.html

**Tenant (1)**

- **HKBU Scholars — Elsevier Pure tenancy** (`x-operator: tenant`) — the research portal and institutional repository. `scholars.hkbu.edu.hk` CNAMEs to `hkbu.elsevierpure.com`. The Pure Web Service answers at `/ws/api` (versioned OpenAPI 401, RapiDoc console 200, OAI-PMH `/ws/oai` 401). The tenancy is a real institutional fact and is recorded as one; the contract is not saved here.
  - Documentation: https://scholars.hkbu.edu.hk/ws/api/rapidoc.html

## Domain standards (education regime)

Recorded in [conformance/hong-kong-baptist-university-conformance.yml](conformance/hong-kong-baptist-university-conformance.yml), every entry backed by a URL and a status code.

| Standard | Conforms | Operator |
|---|---|---|
| `shibboleth` | yes | institution |
| `saml` | yes | institution |
| `lti` | yes | institution |
| `crossref` | yes | institution — member 10204, prefix 10.24112, 1,763 DOIs |
| `oai-pmh` | partial, 401 | tenant — **not credited** |
| `scim`, `orcid`, `datacite`, `oneroster`, `ed-fi`, `caliper`, `qti` | no | — |

## Artifacts

- Conformance: [conformance/hong-kong-baptist-university-conformance.yml](conformance/hong-kong-baptist-university-conformance.yml)
- Authentication: [authentication/hong-kong-baptist-university-authentication.yml](authentication/hong-kong-baptist-university-authentication.yml)
- Domain Security: [security/hong-kong-baptist-university-domain-security.yml](security/hong-kong-baptist-university-domain-security.yml)
- Plans & Pricing: [plans/hong-kong-baptist-university-plans-pricing.yml](plans/hong-kong-baptist-university-plans-pricing.yml)
- Rate Limits: [rate-limits/hong-kong-baptist-university-rate-limits.yml](rate-limits/hong-kong-baptist-university-rate-limits.yml)
- FinOps: [finops/hong-kong-baptist-university-finops.yml](finops/hong-kong-baptist-university-finops.yml)
- Review: [review.yml](review.yml)

There is no `openapi/` directory. HKBU publishes no contract of its own, and the only contract it served was Elsevier's.

## Timestamps

- Created: 2026-06-03
- Modified: 2026-08-30

## Common Properties

- Website: https://www.hkbu.edu.hk/
- Blog: https://www.hkbu.edu.hk/en/whats-new.html
- Identity Federation: https://buidp01.hkbu.edu.hk/idp/shibboleth
- AI Tooling: https://genai.hkbu.edu.hk/
- AI Policy: https://ar.hkbu.edu.hk/student-services/learning-and-teaching/learning-and-teaching-strategy-and-policies/principles-for-the-use-of-generative-ai-tools-in-teaching-and-learning-and-assessment
- Research Repository (tenant): https://scholars.hkbu.edu.hk/
- Institutional Data: https://data-hub.hkbu.edu.hk/
- Terms of Service: https://www.hkbu.edu.hk/en/disclaimer.html
- Privacy Policy: https://bupdpo.hkbu.edu.hk/policies-and-procedures/pps-pics/
- Support: https://ito.hkbu.edu.hk/contact-us.html
- GitHub: https://github.com/HKBUNLP (research-group org; `github.com/hkbu` exists but is empty)
- LinkedIn: https://www.linkedin.com/school/hong-kong-baptist-university/
- Twitter/X: https://twitter.com/hkbaptistu

## Notes

- Every URL in this profile was re-probed on 2026-08-30 with a browser User-Agent. Nothing was fabricated, and status codes — not link presence — decided every entry.
- `www.hkbu.edu.hk` **soft-404s**: `/en/terms-of-use.html`, `/en/privacy-policy.html` and `/en/about-hkbu.html` all return HTTP 200 with `<title>Page not found</title>`. Read the body, not the code. The real terms page is `/en/disclaimer.html`.
- `digital.lib.hkbu.edu.hk` returns a 403 "Access Denied" page to every client tried, including a full browser User-Agent — blocked, not dead.
- The OIRP Data Hub (`data-hub.hkbu.edu.hk`) is live again (it was 503 at the June 2026 review), but it is a link surface over Power BI reports and login-gated sub-apps, with no data API.
- No central institutional developer portal and no institution-wide GitHub organisation exist; only research-group orgs (HKBUNLP, HKBU-HPML) publish code publicly.
- This re-profile removes far more than it adds and is expected to lower the score. That is the correction working: the previous number was Elsevier's engineering credited to a university.

## Maintainers

- Kin Lane — kin@apievangelist.com
