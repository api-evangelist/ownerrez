# OwnerRez (ownerrez)

OwnerRez is vacation-rental and short-term-rental property management software for hosts, owners, and property managers, covering channel management, bookings, guest CRM, quoting, payments, messaging, reviews, and a hosted booking website. The **OwnerRez API v2** is a REST/JSON API served under `https://api.ownerrez.com/v2` that exposes bookings, properties, listings, guests, inquiries, quotes, reviews, guest messaging, payments and financials, custom fields and tags, owners, and outbound webhook subscriptions. Requests are authenticated with an OAuth 2.0 access token (Authorization Code Grant) or with an API key / Personal Access Token supplied as the username in HTTP Basic auth, and server-to-app events are delivered through outbound webhooks. There is no public WebSocket API.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/ownerrez/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/ownerrez/refs/heads/main/apis.yml)

## Tags

- Vacation Rental
- Short-Term Rental
- Property Management
- Hospitality
- Bookings
- Channel Manager

## Timestamps

- **Created:** 2026-07-03
- **Modified:** 2026-07-03

## Authentication

- **OAuth 2.0** — Authorization Code Grant (RFC 6749 §4.1). Authorize at `https://app.ownerrez.com/oauth/authorize`, then exchange the code at `https://api.ownerrez.com/oauth/access_token` (alias `/oauth/token`). Temporary codes expire after 10 minutes.
- **HTTP Basic** — supply your OwnerRez API key / Personal Access Token as the username (blank password).

## Rate Limits

The API is limited to **300 requests per 5 minutes per IP**. Exceeding the limit returns HTTP `429` with a JSON error body; the IP is automatically unblocked once its request rate falls back below the limit.

## APIs

### OwnerRez Bookings API

List, retrieve, create, and update bookings — reservations against a property with arrival/departure dates, guest, occupancy, status, and charge totals.

- **Human URL:** [https://api.ownerrez.com/help/v2](https://api.ownerrez.com/help/v2)
- **Base URL:** `https://api.ownerrez.com/v2`

#### Properties

- [Documentation](https://www.ownerrez.com/support/articles/api-overview)
- [API Reference](https://api.ownerrez.com/help/v2)
- [OpenAPI](openapi/ownerrez-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/ownerrez.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/ownerrez.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### OwnerRez Properties API

Read the rental properties managed in OwnerRez and search them by availability window and occupancy via the PropertySearch endpoint.

- **Human URL:** [https://api.ownerrez.com/help/v2](https://api.ownerrez.com/help/v2)
- **Base URL:** `https://api.ownerrez.com/v2`

### OwnerRez Listings API

Read public listing content (titles, headlines, descriptions) for properties and the channel listing sites — such as Airbnb and Vrbo — that properties are published to.

- **Human URL:** [https://api.ownerrez.com/help/v2](https://api.ownerrez.com/help/v2)
- **Base URL:** `https://api.ownerrez.com/v2`

### OwnerRez Guests API

Manage guest contact records — list, retrieve, create, update, and delete guests, and remove individual addresses, email addresses, and phone numbers from a guest.

- **Human URL:** [https://api.ownerrez.com/help/v2](https://api.ownerrez.com/help/v2)
- **Base URL:** `https://api.ownerrez.com/v2`

### OwnerRez Inquiries API

Read inbound guest inquiries and leads, filtered by property and received time, to feed a lead-management or booking workflow.

- **Human URL:** [https://api.ownerrez.com/help/v2](https://api.ownerrez.com/help/v2)
- **Base URL:** `https://api.ownerrez.com/v2`

### OwnerRez Quotes API

Create, read, update, and delete price quotes for a property and date range, and manage the pricing building blocks that drive them — discounts, fees, surcharges, and ad hoc nightly spot rates.

- **Human URL:** [https://api.ownerrez.com/help/v2](https://api.ownerrez.com/help/v2)
- **Base URL:** `https://api.ownerrez.com/v2`

### OwnerRez Reviews API

Read guest reviews collected for stays and properties, including rating, title, body, and reviewer, for reputation and display use cases.

- **Human URL:** [https://api.ownerrez.com/help/v2](https://api.ownerrez.com/help/v2)
- **Base URL:** `https://api.ownerrez.com/v2`

### OwnerRez Messages API

Read guest message threads and send outbound messages tied to a booking, for automated and manual guest communication.

- **Human URL:** [https://api.ownerrez.com/help/v2](https://api.ownerrez.com/help/v2)
- **Base URL:** `https://api.ownerrez.com/v2`

### OwnerRez Custom Fields and Tags API

Define and apply custom metadata across records — field definitions and their values (Fields/FieldDefinitions) plus tag definitions and their applied tags (Tags/TagDefinitions), including delete-by-definition and delete-by-name helpers.

- **Human URL:** [https://api.ownerrez.com/help/v2](https://api.ownerrez.com/help/v2)
- **Base URL:** `https://api.ownerrez.com/v2`

### OwnerRez Payments and Financials API

Read the financial records attached to bookings — payments, security and damage deposits, and refunds — plus the owners those properties belong to and the authenticated user context.

- **Human URL:** [https://api.ownerrez.com/help/v2](https://api.ownerrez.com/help/v2)
- **Base URL:** `https://api.ownerrez.com/v2`

### OwnerRez Webhook Subscriptions API

Create, list, retrieve, and delete outbound webhook subscriptions and enumerate the available event categories. OwnerRez POSTs event notifications to your subscribed URL; there is no public WebSocket API.

- **Human URL:** [https://www.ownerrez.com/support/articles/api-webhooks](https://www.ownerrez.com/support/articles/api-webhooks)
- **Base URL:** `https://api.ownerrez.com/v2`

## Common Properties

- [GitHub Organization](https://github.com/ownerrez)
- [LinkedIn](https://www.linkedin.com/company/ownerrez)
- [Website](https://www.ownerrez.com)
- [Documentation](https://api.ownerrez.com/help/v2)
- [Plans](plans/ownerrez-plans-pricing.yml)
- [Rate Limits](rate-limits/ownerrez-rate-limits.yml)
- [Fin Ops](finops/ownerrez-finops.yml)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
