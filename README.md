# OwnerRez (ownerrez)

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
