# Not Diamond (notdiamond)

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
