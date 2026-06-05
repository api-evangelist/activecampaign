# ActiveCampaign (activecampaign)

ActiveCampaign is a leading marketing automation platform that helps businesses of all sizes seamlessly engage with their customers. With its user-friendly interface and powerful features, ActiveCampaign allows businesses to create personalized email campaigns, automate workflows, and track customer interactions in real-time. The platform offers a REST API (v3), SMS Broadcast API, webhooks, and custom object schemas for building deep integrations and automations.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/activecampaign/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/activecampaign/refs/heads/main/apis.yml)

## Scope

- **Type:** Index
- **Position:** Consumer
- **Access:** 3rd-Party

## Tags

- Marketing Automation
- Email Marketing
- CRM
- Sales Automation
- Customer Experience

## Timestamps

- **Created:** 2025-02-17
- **Modified:** 2026-05-30

## APIs

### ActiveCampaign API v3

The primary REST API for ActiveCampaign, organized around resources such as contacts, deals, accounts, automations, campaigns, messages, lists, tags, webhooks, custom objects, and ecommerce entities. Uses API key header authentication.

- **Human URL:** [https://developers.activecampaign.com/reference/overview](https://developers.activecampaign.com/reference/overview)
- **Base URL:** `https://youraccountname.api-us1.com/api/3`

#### Tags

- Marketing Automation
- CRM
- Email Marketing
- Contacts
- Deals

#### Properties

- [Documentation](https://developers.activecampaign.com/reference/overview)
- [Authentication](https://developers.activecampaign.com/reference/authentication)
- [OpenAPI](openapi/activecampaign-v3.json) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/activecampaign-v3.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/activecampaign-v3.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [AsyncAPI](asyncapi/activecampaign-webhooks-asyncapi.yml) — [AsyncAPI Specification](https://www.asyncapi.com/docs/reference/specification/latest)

### ActiveCampaign SMS Broadcast API

API for managing SMS broadcasts, lists, metrics, and AI-powered content generation in ActiveCampaign. Supports creating, scheduling, and tracking SMS broadcast campaigns.

- **Human URL:** [https://developers.activecampaign.com/reference/overview](https://developers.activecampaign.com/reference/overview)
- **Base URL:** `https://youraccountname.api-us1.com/api/3`

#### Tags

- SMS
- Marketing Automation
- Messaging

#### Properties

- [Documentation](https://developers.activecampaign.com/reference/overview)
- [OpenAPI](openapi/activecampaign-sms.json) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/activecampaign-sms.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/activecampaign-sms.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [JSON Schema](json-schema/activecampaign-sms-broadcast-message-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/activecampaign-sms-broadcast-create-request-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/activecampaign-sms-broadcast-update-request-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/activecampaign-sms-broadcast-metrics-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/activecampaign-sms-recipient-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/activecampaign-sms-credits-response-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/activecampaign-sms-ai-broadcast-request-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Structure](json-structure/activecampaign-sms-broadcast-message-structure.json)
- [JSON Structure](json-structure/activecampaign-sms-recipient-structure.json)
- [Example](examples/activecampaign-sms-broadcast-message-example.json)
- [Example](examples/activecampaign-sms-recipient-example.json)

## Common Properties

- [Arazzo Workflows](arazzo/) — [Arazzo Specification](https://spec.openapis.org/arazzo/latest.html)
- [LinkedIn](https://www.linkedin.com/company/activecampaign)
- [Portal](https://developers.activecampaign.com/)
- [Getting Started](https://help.activecampaign.com/hc/en-us/articles/207317590-Getting-started-with-the-API)
- [Authentication](https://developers.activecampaign.com/reference/authentication)
- [Pricing](https://www.activecampaign.com/pricing)
- [Blog](https://www.activecampaign.com/blog)
- [F A Q](https://www.activecampaign.com/about/faq)
- [Forums](https://community.activecampaign.com/latest)
- [Status Page](https://status.activecampaign.com/)
- [Postman Workspace](https://www.postman.com/acdevrel/activecampaign-developer-relations/overview)
- [GitHub Organization](https://github.com/ActiveCampaign)
- [SDK](https://github.com/ActiveCampaign/activecampaign-api-php)
- [SDK](https://github.com/ActiveCampaign/activecampaign-api-nodejs)
- [Spectral Rules](rules/activecampaign-spectral-rules.yml)
- [Vocabulary](vocabulary/activecampaign-vocabulary.yaml)
- [JSON-LD](json-ld/activecampaign-sms-context.jsonld) — [JSON-LD](https://www.w3.org/TR/json-ld11/)
- [Features](undefined)
- [Use Cases](undefined)
- [Integrations](undefined)
- [Solutions](undefined)
- [M C P Server](https://github.com/ActiveCampaign/postmark-mcp)
- [Agent Skill](https://github.com/ActiveCampaign/postmark-skills)
- [L L Ms Txt](https://developers.activecampaign.com/llms.txt)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
