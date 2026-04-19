# ActiveCampaign (activecampaign)
ActiveCampaign is a leading marketing automation platform that helps businesses of all sizes seamlessly engage with their customers. With its user-friendly interface and powerful features, ActiveCampaign allows businesses to create personalized email campaigns, automate workflows, and track customer interactions in real-time. The platform offers a REST API (v3), SMS Broadcast API, webhooks, and custom object schemas for building deep integrations and automations.

**URL:** [https://developers.activecampaign.com/](https://developers.activecampaign.com/)

**Run:** [Capabilities Using Naftiko](https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=company-api-evangelist&utm_content=repo)

## Tags:

 - Marketing Automation, Email Marketing, CRM, Sales Automation, Customer Experience

## Timestamps

- **Created:** 2025-02-17
- **Modified:** 2026-04-19

## APIs

### ActiveCampaign API v3
The primary REST API for ActiveCampaign, organized around resources such as contacts, deals, accounts, automations, campaigns, messages, lists, tags, webhooks, custom objects, and ecommerce entities. Uses API key header authentication.

**Human URL:** [https://developers.activecampaign.com/reference/overview](https://developers.activecampaign.com/reference/overview)

#### Tags:

 - Marketing Automation, CRM, Email Marketing, Contacts, Deals

#### Properties

- [Documentation](https://developers.activecampaign.com/reference/overview)
- [Authentication](https://developers.activecampaign.com/reference/authentication)
- [OpenAPI](openapi/activecampaign-v3.json)

### ActiveCampaign SMS Broadcast API
API for managing SMS broadcasts, lists, metrics, and AI-powered content generation in ActiveCampaign. Supports creating, scheduling, and tracking SMS broadcast campaigns.

**Human URL:** [https://developers.activecampaign.com/reference/overview](https://developers.activecampaign.com/reference/overview)

#### Tags:

 - SMS, Marketing Automation, Messaging

#### Properties

- [Documentation](https://developers.activecampaign.com/reference/overview)
- [OpenAPI](openapi/activecampaign-sms.json)
- [JSONSchema - Broadcast Message](json-schema/activecampaign-sms-broadcast-message-schema.json)
- [JSONSchema - Broadcast Create Request](json-schema/activecampaign-sms-broadcast-create-request-schema.json)
- [JSONSchema - Recipient](json-schema/activecampaign-sms-recipient-schema.json)
- [JSONStructure - Broadcast Message](json-structure/activecampaign-sms-broadcast-message-structure.json)
- [Example - Broadcast Message](examples/activecampaign-sms-broadcast-message-example.json)

## Common Properties

- [Portal](https://developers.activecampaign.com/)
- [GettingStarted](https://help.activecampaign.com/hc/en-us/articles/207317590-Getting-started-with-the-API)
- [Authentication](https://developers.activecampaign.com/reference/authentication)
- [Pricing](https://www.activecampaign.com/pricing)
- [Blog](https://www.activecampaign.com/blog)
- [FAQ](https://www.activecampaign.com/about/faq)
- [Forums](https://community.activecampaign.com/latest)
- [StatusPage](https://status.activecampaign.com/)
- [PostmanWorkspace](https://www.postman.com/acdevrel/activecampaign-developer-relations/overview)
- [GitHubOrganization](https://github.com/ActiveCampaign)
- [SDK - PHP SDK](https://github.com/ActiveCampaign/activecampaign-api-php)
- [SDK - Node.js SDK](https://github.com/ActiveCampaign/activecampaign-api-nodejs)

## Features

| Name | Description |
|------|-------------|
| Email Marketing | Create and send conversion-focused email campaigns with personalization and segmentation. |
| Marketing Automation | Build automated customer journeys and workflows triggered by contact behavior and events. |
| CRM | Built-in sales CRM for managing deals, pipelines, tasks, and customer relationships. |
| SMS Marketing | Reach contacts via SMS broadcast campaigns with AI-powered content generation. |
| WhatsApp Messaging | Automate growth and customer engagement through WhatsApp communications. |
| Transactional Email | Automate transactional alerts, password resets, and notifications via Postmark integration. |
| Custom Objects | Create custom data schemas to activate complex data for segmentation and personalized automation. |
| Contact Event Tracking | Track contact behaviors and activities across web properties and integrations. |
| Webhooks | Receive real-time event notifications for contact, campaign, automation, and custom object activities. |
| Landing Pages | Deploy conversion-ready landing pages for lead capture and campaigns. |
| Active Intelligence | AI-powered orchestration and autonomous marketing agents for campaign suggestions and personalization. |
| MCP Server | Connect AI applications to ActiveCampaign using the Model Context Protocol server. |

## Use Cases

| Name | Description |
|------|-------------|
| Lead Nurturing | Automate email sequences to nurture leads through the sales funnel based on behavior. |
| E-Commerce Automation | Trigger post-purchase emails, abandoned cart recovery, and personalized product recommendations. |
| Customer Onboarding | Automate onboarding sequences for SaaS products to improve activation and retention. |
| Contact Segmentation | Segment contacts using tags, custom fields, and custom objects for targeted campaigns. |
| Sales Pipeline Management | Manage deals, tasks, and pipeline stages with CRM and automation integration. |
| SMS Broadcast Campaigns | Send targeted SMS campaigns to subscriber lists with engagement tracking. |
| Webhook-Driven Integrations | Build real-time integrations using webhooks for contact and campaign activity events. |

## Integrations

| Name | Description |
|------|-------------|
| Salesforce | Sync contact and deal data between ActiveCampaign and Salesforce CRM. |
| Zapier | Connect ActiveCampaign to 1000+ apps via Zapier automation workflows. |
| Slack | Send notifications and trigger automations from Slack using OAuth2 integration. |
| Calendly | Sync scheduling data and trigger automations with custom objects via OAuth2. |
| Twilio | Integrate SMS workflows using Twilio with Basic Auth for outbound messaging. |
| Shopify | Sync ecommerce customers, orders, and products for automated campaigns. |
| WordPress | Embed forms and capture leads from WordPress sites. |
| Wix | Connect Wix websites for lead capture and customer journey automation. |

## Solutions

| Name | Description |
|------|-------------|
| Starter | Entry-level plan with marketing automation, up to 5 automation actions, and 1 user. |
| Plus | Mid-tier plan with unlimited automation actions, landing pages, and standard segmentation. |
| Pro | Advanced plan with predictive content, advanced segmentation, and 3 users. |
| Enterprise | Full-featured plan with custom objects, dedicated account team, and premium segmentation. |

## Artifacts

Machine-readable API specifications organized by format.

### OpenAPI

- [ActiveCampaign API v3](openapi/activecampaign-v3.json)
- [ActiveCampaign SMS Broadcast API](openapi/activecampaign-sms.json)

### JSON Schema

- [Broadcast Message](json-schema/activecampaign-sms-broadcast-message-schema.json)
- [Broadcast Create Request](json-schema/activecampaign-sms-broadcast-create-request-schema.json)
- [Broadcast Update Request](json-schema/activecampaign-sms-broadcast-update-request-schema.json)
- [Broadcast Metrics](json-schema/activecampaign-sms-broadcast-metrics-schema.json)
- [Recipient](json-schema/activecampaign-sms-recipient-schema.json)
- [Credits Response](json-schema/activecampaign-sms-credits-response-schema.json)
- [AI Broadcast Request](json-schema/activecampaign-sms-ai-broadcast-request-schema.json)
- [AI Broadcast Status](json-schema/activecampaign-sms-ai-broadcast-status-schema.json)

### JSON Structure

- [Broadcast Message](json-structure/activecampaign-sms-broadcast-message-structure.json)
- [Recipient](json-structure/activecampaign-sms-recipient-structure.json)
- [Credits Response](json-structure/activecampaign-sms-credits-response-structure.json)
- [Broadcast Metrics](json-structure/activecampaign-sms-broadcast-metrics-structure.json)

### JSON-LD

- [ActiveCampaign SMS Context](json-ld/activecampaign-sms-context.jsonld)

### Examples

- [Broadcast Message](examples/activecampaign-sms-broadcast-message-example.json)
- [Recipient](examples/activecampaign-sms-recipient-example.json)
- [Credits Response](examples/activecampaign-sms-credits-response-example.json)

## Capabilities

Naftiko capabilities organized as shared per-API definitions composed into customer-facing workflows.

### Shared Per-API Definitions

- [ActiveCampaign API v3](capabilities/shared/activecampaign-v3.yaml) — 17 operations for contacts, deals, accounts, automations, campaigns, lists, tags, and webhooks

### Workflow Capabilities

| Workflow | APIs Combined | Tools | Persona |
|----------|--------------|-------|---------|
| [Marketing Automation](capabilities/marketing-automation.yaml) | ActiveCampaign v3 | 8 | Marketing Manager, Growth Engineer |
| [CRM and Sales](capabilities/crm-sales.yaml) | ActiveCampaign v3 | 5 | Sales Representative, Revenue Operations |

## Vocabulary

- [ActiveCampaign Vocabulary](vocabulary/activecampaign-vocabulary.yaml) — Unified taxonomy mapping 13 resources, 7 actions, 2 workflows, and 3 personas across operational (OpenAPI) and capability (Naftiko) dimensions

## Rules

- [activecampaign-spectral-rules.yml](rules/activecampaign-spectral-rules.yml) — 22 rules across 8 categories enforcing ActiveCampaign API conventions

## Maintainers

**FN:** Kin Lane

**Email:** kin@apievangelist.com
