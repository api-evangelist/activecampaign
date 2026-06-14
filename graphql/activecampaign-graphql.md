# ActiveCampaign GraphQL Schema

## Overview

ActiveCampaign provides a REST API (v3) for customer experience automation, marketing automation, CRM, and email marketing. This conceptual GraphQL schema represents the core domain model of the ActiveCampaign platform, translating its REST resources into a unified, queryable graph structure.

ActiveCampaign does not expose a native GraphQL endpoint. This schema is a conceptual translation of the REST API surface documented at https://developers.activecampaign.com/reference/overview, intended to illustrate the relationships between platform resources and support tooling that benefits from a typed graph representation.

## Source API

- **API Version**: v3
- **Base URL**: `https://{account}.api-us1.com/api/3`
- **Authentication**: API key via `Api-Token` header
- **Documentation**: https://developers.activecampaign.com/reference/overview

## Schema Design Notes

### Root Types

The schema defines three root operation types:

- **Query**: Read operations across all resource types
- **Mutation**: Create, update, and delete operations
- **Subscription**: Real-time event notifications (conceptual; mapped from webhook event types)

### Core Domain Areas

**Contact Management**
Contacts are the central entity. Each contact can have tags, custom field values, list subscriptions, scores, and notes. Contacts are associated with accounts (organizations) via the `AccountContact` join type.

**Marketing Automation**
Automations represent multi-step customer journeys. `ContactAutomation` tracks a specific contact's enrollment status in an automation. Goals are checkpoints within automations.

**Email Campaigns**
Campaigns represent email sends to lists or segments. Messages are the email content templates. Reports surface aggregate performance metrics per campaign.

**CRM / Deals**
Deals represent sales opportunities and belong to a pipeline and stage. Each deal can have tasks, notes, contacts, and custom field values. `DealPipeline` and `DealStage` model the sales funnel structure.

**Lists and Segmentation**
Lists are subscription groups. Segments are dynamic filters. Tags are freeform labels applied to contacts. Scores are numeric values calculated from contact behavior.

**Conversations and Messaging**
Conversations aggregate inbound and outbound messages across channels. `ConversationMessage` represents individual messages within a conversation thread.

**Tracking**
`SiteTracking` manages web property tracking configuration. `EventTracking` handles custom event definitions. `EventLog` records individual tracking events per contact.

**Webhooks and Integrations**
Webhooks deliver real-time POST payloads to external URLs when specific events occur. Integrations represent connected third-party applications.

**Templates**
Templates define reusable email designs composed of `TemplateBlock` sections.

**Users and Permissions**
Users are platform members. Groups are collections of users. Permissions control feature access per user or group.

## Type Summary

| Category | Types |
|---|---|
| Contacts | Contact, ContactTag, ContactAutomation, FieldValue, CustomField, Score, Segment |
| Accounts | Account, AccountContact |
| Automation | Automation, Goal |
| Campaigns | Campaign, Template, TemplateBlock |
| Messaging | Email, Message, Conversation, ConversationMessage, Chat, BrandedLink, Bounce |
| Lists | List, Subscription, Form |
| CRM | Deal, DealPipeline, DealStage, DealContact, Task, Note, Activity |
| Tracking | SiteTracking, EventTracking, EventLog, Tracking |
| Tags | Tag |
| Users | User, Group, Permission |
| Reporting | Report |
| Webhooks | Webhook, ImportStatus |
| Calendar | CalendarFeed |

## Relationships

- `Contact` has many `Tag` (via `ContactTag`), `List` (via `Subscription`), `FieldValue`, `Note`, `Activity`, `ContactAutomation`, `Score`
- `Contact` belongs to many `Account` (via `AccountContact`)
- `Deal` belongs to `DealPipeline` and `DealStage`; has many `Task`, `Note`, `DealContact`, `FieldValue`
- `Automation` has many `Goal`; contacts enroll via `ContactAutomation`
- `Campaign` references a `List`, `Message`, and produces a `Report`
- `Conversation` has many `ConversationMessage`
- `Template` has many `TemplateBlock`
- `User` belongs to many `Group`; `Group` has many `Permission`

## Scalar Types

- `ID`: Unique identifier
- `String`: UTF-8 text
- `Int`: Integer number
- `Float`: Floating-point number
- `Boolean`: True or false
- `DateTime`: ISO 8601 timestamp string
- `JSON`: Arbitrary JSON value (for custom fields, metadata)
- `URL`: Absolute URL string

## Usage Notes

This schema is conceptual and not backed by a live GraphQL endpoint. It may be used to:

- Generate mock servers for testing integrations
- Produce documentation and data dictionaries
- Drive code generation tooling for type-safe clients
- Inform federation or API gateway layer designs that sit atop the ActiveCampaign REST API
