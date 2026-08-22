# Not Diamond (notdiamond)

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

Not Diamond is an AI model router that determines the best LLM to call for any given prompt. Its REST API routes each request to the optimal model across providers based on quality, cost, and latency tradeoffs, accepts real-time feedback to personalize routing, and can train custom routers from evaluation datasets.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/notdiamond/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/notdiamond/refs/heads/main/apis.yml)

## Tags

- AI
- LLM
- Model Routing
- Router
- Orchestration

## Timestamps

- **Created:** 2026-06-20
- **Modified:** 2026-06-20

## APIs

### Not Diamond Model Select API

Routes a prompt to the best available LLM. Submit OpenAI-format messages and a list of candidate providers, and the modelSelect endpoint returns the recommended provider/model plus a session ID, honoring cost/latency/quality tradeoffs and an optional preference ID for personalized or custom routing.

- **Human URL:** [https://docs.notdiamond.ai/reference/token_model_select_v2_modelrouter_modelselect_post](https://docs.notdiamond.ai/reference/token_model_select_v2_modelrouter_modelselect_post)
- **Base URL:** `https://api.notdiamond.ai/v2`

#### Tags

- Model Routing
- Model Select
- Routing
- LLM

#### Properties

- [Documentation](https://docs.notdiamond.ai/docs/quickstart)
- [API Reference](https://docs.notdiamond.ai/reference/token_model_select_v2_modelrouter_modelselect_post)
- [OpenAPI](openapi/notdiamond-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/notdiamond.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/notdiamond.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Not Diamond Models API

Lists supported text generation models with provider, context length, and per-million-token input/output pricing, with optional filtering by provider or OpenRouter support.

- **Human URL:** [https://docs.notdiamond.ai/reference/list_models_v2_models_get](https://docs.notdiamond.ai/reference/list_models_v2_models_get)
- **Base URL:** `https://api.notdiamond.ai/v2`

#### Tags

- Models
- Catalog

#### Properties

- [API Reference](https://docs.notdiamond.ai/reference/list_models_v2_models_get)
- [OpenAPI](openapi/notdiamond-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/notdiamond.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/notdiamond.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Not Diamond Feedback API

Reports outcome feedback and latency metrics against a routing session so Not Diamond can continuously personalize routing decisions in real time to an application's end users.

- **Human URL:** [https://docs.notdiamond.ai/docs/real-time-personalization](https://docs.notdiamond.ai/docs/real-time-personalization)
- **Base URL:** `https://api.notdiamond.ai/v2`

#### Tags

- Feedback
- Personalization
- Metrics

#### Properties

- [Documentation](https://docs.notdiamond.ai/docs/real-time-personalization)
- [OpenAPI](openapi/notdiamond-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/notdiamond.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/notdiamond.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Not Diamond Custom Routers API

Trains a custom router from an uploaded CSV evaluation dataset and creates or updates a user preference, returning a preference ID used to drive personalized routing in subsequent modelSelect calls.

- **Human URL:** [https://docs.notdiamond.ai/reference/train_custom_router_v2_pzn_traincustomrouter_post](https://docs.notdiamond.ai/reference/train_custom_router_v2_pzn_traincustomrouter_post)
- **Base URL:** `https://api.notdiamond.ai/v2`

#### Tags

- Custom Routers
- Training
- Personalization

#### Properties

- [API Reference](https://docs.notdiamond.ai/reference/train_custom_router_v2_pzn_traincustomrouter_post)
- [OpenAPI](openapi/notdiamond-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/notdiamond.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/notdiamond.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [GitHub Organization](https://github.com/Not-Diamond)
- [LinkedIn](https://www.linkedin.com/company/not-diamond)
- [Website](https://www.notdiamond.ai)
- [Documentation](https://docs.notdiamond.ai)
- [Plans](plans/notdiamond-plans-pricing.yml)
- [Rate Limits](rate-limits/notdiamond-rate-limits.yml)
- [Fin Ops](finops/notdiamond-finops.yml)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
