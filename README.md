# Hong Kong Baptist University

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

Hong Kong Baptist University (HKBU) is a publicly funded, UGC-supported research university in Hong Kong SAR. Re-profiled on 2026-08-30 under the API Evangelist university pipeline, which settles WHO OPERATES each surface before crediting any contract. HKBU operates no central developer portal, no public API catalogue and no institution-wide GitHub organisation; github.com/hkbu exists but is empty, and the only active HKBU orgs are research labs (HKBUNLP, HKBU-HPML). What HKBU does operate itself, verified by live probe, is four things: a Shibboleth/SAML 2.0 identity provider at buidp01.hkbu.edu.hk registered in eduGAIN through the Hong Kong Access Federation since 2018 and serving 12KB of signed SAML metadata anonymously; a self-built GenAI Platform whose Azure-OpenAI-shaped chat-completions and embeddings endpoints answer on genai.hkbu.edu.hk behind an api-key header, undocumented publicly; a self-hosted Moodle at buelearning.hkbu.edu.hk publishing a live IMS LTI 1.3 JWKS and OAuth2 token endpoint under HKBU's own signing keys; and a first-party mobile-app backend at mapp-api.hkbu.edu.hk with no public documentation. Everything that looks like an HKBU research API is not. The HKBU Scholars portal at scholars.hkbu.edu.hk is a CNAME to hkbu.elsevierpure.com — an Elsevier Pure tenancy. The 33 OpenAPI documents previously held in this repository were Elsevier's Pure Web Service contract 5.35.0 (info.contact pure-support@elsevier.com), the same document other Pure institutions ship, and have been removed along with everything derived from them. The data is HKBU's; the contract is Elsevier's, and it scores in Elsevier's repository, not here.

**Areas:** University · Higher Education · Education · Hong Kong · UGC-Funded · Identity Federation · Shibboleth · SAML · eduGAIN · LMS · LTI · Artificial Intelligence

## Hong Kong Baptist University on APIs.io

Everything profiled for Hong Kong Baptist University is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/hong-kong-baptist-university/](https://apis.io/providers/hong-kong-baptist-university/)** — or go straight to one of the APIs or properties below.

### APIs (5)

- [HKBU Identity Federation (Shibboleth IdP / SAML 2.0 metadata)](https://apis.io/apis/hong-kong-baptist-university/identity-federation/) — HKBU's own SAML 2.0 identity provider, entityID https://buidp01.hkbu.edu.hk/idp/shibboleth, registered in eduGAIN by the Hong Kong Access Federation (HKAF)…
- [HKBU GenAI Platform API (undocumented, key-gated)](https://apis.io/apis/hong-kong-baptist-university/genai-platform-api/) — HKBU runs its own generative-AI gateway at genai.hkbu.edu.hk, fronting third-party models (Anthropic, Google, Meta AI, OpenAI) for staff and students.…
- [HKBU Moodle — IMS LTI 1.3 platform + web services](https://apis.io/apis/hong-kong-baptist-university/moodle-lti-platform/) — HKBU self-hosts Moodle at buelearning.hkbu.edu.hk on its own registrable domain. It publishes a live IMS LTI 1.3 Advantage tool-platform key set at…
- [HKBU Mobile App Backend (gated)](https://apis.io/apis/hong-kong-baptist-university/mobile-app-backend/) — Backend host serving the official HKBU Mobile application (mapp-api.hkbu.edu.hk). The host resolves over TLS 1.3 with HSTS and serves app support content…
- [HKBU Scholars — Elsevier Pure tenancy (tenant relationship, contract not HKBU's)](https://apis.io/apis/hong-kong-baptist-university/scholars-pure-tenancy/) — HKBU Scholars is HKBU's research information portal and institutional repository, and it is an Elsevier Pure tenancy: scholars.hkbu.edu.hk is a CNAME to…

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### Vocabulary (1)

The provider's domain terms, defined.

- [HKBU Scholars Pure Web Service Vocabulary](https://apis.io/vocabularies/hong-kong-baptist-university/hong-kong-baptist-university-vocabulary/)

#### Security (2)

Authentication, trust centre, and vulnerability disclosure.

- [Hong Kong Baptist University Authentication](https://apis.io/security/hong-kong-baptist-university/hong-kong-baptist-university-authentication/)
- [Hong Kong Baptist University Domain Security](https://apis.io/security/hong-kong-baptist-university/hong-kong-baptist-university-domain-security/)

#### Plans and pricing (1)

Published plans, tiers and prices.

- [Hong Kong Baptist University Plans Pricing](https://apis.io/plans/hong-kong-baptist-university/hong-kong-baptist-university-plans-pricing/)

#### Rate limits (1)

Published request limits.

- [Hong Kong Baptist University Rate Limits](https://apis.io/rate-limits/hong-kong-baptist-university/hong-kong-baptist-university-rate-limits/)

#### FinOps (1)

What the API costs to run, by operation.

- [Hong Kong Baptist University Finops](https://apis.io/finops/hong-kong-baptist-university/hong-kong-baptist-university-finops/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://www.hkbu.edu.hk/)
- [Support](https://ito.hkbu.edu.hk/contact-us.html)
- [Blog](https://www.hkbu.edu.hk/en/whats-new.html)
- [Terms of service](https://www.hkbu.edu.hk/en/disclaimer.html)
- [Privacy policy](https://bupdpo.hkbu.edu.hk/policies-and-procedures/pps-pics/)

## API Evangelist rating

**Kin Score 23.6** — emerging · rubric 0.24.0 · scored 2026-10-17

| Facet | Score |
|---|---|
| Discoverability | 62.5 |
| Contract quality | 4.4 |
| Contract governance | 18.2 |
| Operational transparency | 10.5 |
| Developer ergonomics | 28.6 |
| Access clarity | 26.3 |

**Agent readiness 3.1** — human-only

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | — |
| Agentic Access | — |
| Reversibility Documented | — |
| MCP Server | — |
| Auth Clarity | bearer (partial credit) |
| Idempotency | — |
| Error Semantics | — |
| OpenAPI Examples | — |
| Rate Limit Signal | derived (partial credit) |
| Event Surface Described | — |
| Agent Skills | — |
| Well Known Catalog | — |
| Consent Identity | — |
| Agent Card | — |
| Dry Run Mode | — |
| Delegated Identity | — |
| Protected Resource Metadata | — |
| Dynamic Client Registration | — |
| Agentic Commerce | — |

**Regulatory alignment 30.0** — Education & Research

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/hong-kong-baptist-university/](https://apis.io/providers/hong-kong-baptist-university/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for Hong Kong Baptist University: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/hong-kong-baptist-university/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
