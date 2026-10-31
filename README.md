# OwnerRez

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

OwnerRez is vacation-rental and short-term-rental property management software for hosts, owners, and property managers, covering channel management, bookings, guest CRM, quoting, payments, messaging, reviews, and a hosted booking website. The OwnerRez API v2 is a REST/JSON API served under https://api.ownerrez.com/v2 that exposes bookings, properties, listings, guests, inquiries, quotes, reviews, guest messaging, payments and financials, custom fields and tags, owners, and outbound webhook subscriptions. Requests are authenticated with an OAuth 2.0 access token (Authorization Code Grant) or with an API key / Personal Access Token via HTTP Basic auth, and server-to-app events are delivered through outbound webhooks.

**Areas:** Vacation Rentals · Short-Term Rental · Property Management · Hospitality · Booking · Channel Manager

## OwnerRez on APIs.io

Everything profiled for OwnerRez is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/ownerrez/](https://apis.io/providers/ownerrez/)** — or go straight to one of the APIs or properties below.

### APIs (23)

- [OwnerRez Bookings API](https://apis.io/apis/ownerrez/ownerrez-bookings-api/) — Reservations against a property, including dates, guest, and charges.
- [OwnerRez Deposits API](https://apis.io/apis/ownerrez/ownerrez-deposits-api/) — Security and damage deposits.
- [OwnerRez Discounts API](https://apis.io/apis/ownerrez/ownerrez-discounts-api/) — Discount rules.
- [OwnerRez Fees API](https://apis.io/apis/ownerrez/ownerrez-fees-api/) — Fees applied to bookings and quotes.
- [OwnerRez Fields API](https://apis.io/apis/ownerrez/ownerrez-fields-api/) — Custom field values attached to records.
- [OwnerRez Guests API](https://apis.io/apis/ownerrez/ownerrez-guests-api/) — Guest contact records and their addresses, emails, and phones.
- [OwnerRez Inquiries API](https://apis.io/apis/ownerrez/ownerrez-inquiries-api/) — Inbound guest inquiries and leads.
- [OwnerRez Listings API](https://apis.io/apis/ownerrez/ownerrez-listings-api/) — Public listing content and channel listing sites for properties.
- [OwnerRez Messages API](https://apis.io/apis/ownerrez/ownerrez-messages-api/) — Guest messaging threads and outbound messages.
- [OwnerRez Owners API](https://apis.io/apis/ownerrez/ownerrez-owners-api/) — Property owners.
- [OwnerRez Payments API](https://apis.io/apis/ownerrez/ownerrez-payments-api/) — Payments recorded against bookings.
- [OwnerRez Properties API](https://apis.io/apis/ownerrez/ownerrez-properties-api/) — Rental properties managed in OwnerRez.
- [OwnerRez Quotes API](https://apis.io/apis/ownerrez/ownerrez-quotes-api/) — Price quotes generated for a stay.
- [OwnerRez Refunds API](https://apis.io/apis/ownerrez/ownerrez-refunds-api/) — Refunds issued against payments.
- [OwnerRez Reviews API](https://apis.io/apis/ownerrez/ownerrez-reviews-api/) — Guest reviews collected for stays and properties.
- [OwnerRez SpotRates API](https://apis.io/apis/ownerrez/ownerrez-spotrates-api/) — Ad hoc nightly spot-rate overrides.
- [OwnerRez Surcharges API](https://apis.io/apis/ownerrez/ownerrez-surcharges-api/) — Surcharge rules applied to bookings and quotes.
- [OwnerRez TagDefinitions API](https://apis.io/apis/ownerrez/ownerrez-tagdefinitions-api/) — Definitions of tags.
- [OwnerRez Tags API](https://apis.io/apis/ownerrez/ownerrez-tags-api/) — Tag values applied to records.
- [OwnerRez Users API](https://apis.io/apis/ownerrez/ownerrez-users-api/) — The authenticated user context.
- [OwnerRez Field Definitions API](https://apis.io/apis/ownerrez/ownerrez-field-definitions-api/) — Definitions of custom fields.
- [OwnerRez Property Search API](https://apis.io/apis/ownerrez/ownerrez-property-search-api/) — Availability and criteria search across properties.
- [OwnerRez Webhook Subscriptions API](https://apis.io/apis/ownerrez/ownerrez-webhook-subscriptions-api/) — Outbound webhook subscriptions and their event categories.

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### Agentic access (1)

Which operations an agent can call, which act, and which need a human in the loop.

- [Ownerrez Agentic Access](https://apis.io/agentic-access/ownerrez/ownerrez-agentic-access/)

#### Collections (23)

Postman and Open Collection request collections.

- [OwnerRez API v2](https://apis.io/collections/ownerrez/open-ownerrez/)
- [OwnerRez API v2 Bookings API](https://apis.io/collections/ownerrez/open-ownerrez-bookings-api/)
- [OwnerRez API v2 Bookings Deposits API](https://apis.io/collections/ownerrez/open-ownerrez-deposits-api/)
- [OwnerRez API v2 Bookings Discounts API](https://apis.io/collections/ownerrez/open-ownerrez-discounts-api/)
- [OwnerRez API v2 Bookings Fees API](https://apis.io/collections/ownerrez/open-ownerrez-fees-api/)
- [OwnerRez API v2 Bookings FieldDefinitions API](https://apis.io/collections/ownerrez/open-ownerrez-fielddefinitions-api/)
- [OwnerRez API v2 Bookings Fields API](https://apis.io/collections/ownerrez/open-ownerrez-fields-api/)
- [OwnerRez API v2 Bookings Guests API](https://apis.io/collections/ownerrez/open-ownerrez-guests-api/)
- [OwnerRez API v2 Bookings Inquiries API](https://apis.io/collections/ownerrez/open-ownerrez-inquiries-api/)
- [OwnerRez API v2 Bookings Listings API](https://apis.io/collections/ownerrez/open-ownerrez-listings-api/)
- [OwnerRez API v2 Bookings Messages API](https://apis.io/collections/ownerrez/open-ownerrez-messages-api/)
- [OwnerRez API v2 Bookings Owners API](https://apis.io/collections/ownerrez/open-ownerrez-owners-api/)
- [OwnerRez API v2 Bookings Payments API](https://apis.io/collections/ownerrez/open-ownerrez-payments-api/)
- [OwnerRez API v2 Bookings Properties API](https://apis.io/collections/ownerrez/open-ownerrez-properties-api/)
- [OwnerRez API v2 Bookings PropertySearch API](https://apis.io/collections/ownerrez/open-ownerrez-propertysearch-api/)
- [OwnerRez API v2 Bookings Quotes API](https://apis.io/collections/ownerrez/open-ownerrez-quotes-api/)
- [OwnerRez API v2 Bookings Refunds API](https://apis.io/collections/ownerrez/open-ownerrez-refunds-api/)
- [OwnerRez API v2 Bookings SpotRates API](https://apis.io/collections/ownerrez/open-ownerrez-spotrates-api/)
- [OwnerRez API v2 Bookings Surcharges API](https://apis.io/collections/ownerrez/open-ownerrez-surcharges-api/)
- [OwnerRez API v2 Bookings TagDefinitions API](https://apis.io/collections/ownerrez/open-ownerrez-tagdefinitions-api/)
- [OwnerRez API v2 Bookings Tags API](https://apis.io/collections/ownerrez/open-ownerrez-tags-api/)
- [OwnerRez API v2 Bookings Users API](https://apis.io/collections/ownerrez/open-ownerrez-users-api/)
- [OwnerRez API v2 Bookings WebhookSubscriptions API](https://apis.io/collections/ownerrez/open-ownerrez-webhooksubscriptions-api/)

#### Security (2)

Authentication, trust centre, and vulnerability disclosure.

- [Ownerrez Authentication](https://apis.io/security/ownerrez/ownerrez-authentication/)
- [Ownerrez Domain Security](https://apis.io/security/ownerrez/ownerrez-domain-security/)

#### OAuth scopes (1)

The permissions the API asks for.

- [Ownerrez Scopes](https://apis.io/scopes/ownerrez/ownerrez-scopes/)

#### Plans and pricing (1)

Published plans, tiers and prices.

- [Ownerrez Plans Pricing](https://apis.io/plans/ownerrez/ownerrez-plans-pricing/)

#### Rate limits (1)

Published request limits.

- [Ownerrez Rate Limits](https://apis.io/rate-limits/ownerrez/ownerrez-rate-limits/)

#### FinOps (1)

What the API costs to run, by operation.

- [Ownerrez Finops](https://apis.io/finops/ownerrez/ownerrez-finops/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://www.ownerrez.com)
- [Documentation](https://api.ownerrez.com/help/v2)
- [Blog](https://www.ownerrez.com/blog)
- [GitHub](https://github.com/ownerrez)

## API Evangelist rating

**Kin Score 28.7** — thin · rubric 0.24.0 · scored 2026-10-17

| Facet | Score |
|---|---|
| Discoverability | 66.1 |
| Contract quality | 52.1 |
| Contract governance | 0.0 |
| Operational transparency | 7.9 |
| Developer ergonomics | 31.0 |
| Access clarity | 7.9 |

**Agent readiness 24.7** — agent-aware

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | yes |
| Agentic Access | derived (partial credit) |
| Reversibility Documented | documented (partial credit) |
| MCP Server | — |
| Auth Clarity | negotiable (partial credit) |
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
| Delegated Identity | documented (partial credit) |
| Protected Resource Metadata | — |
| Dynamic Client Registration | — |
| Agentic Commerce | — |

**Regulatory alignment 21.6** — Horizontal (data, software, accessibility, platform)

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/ownerrez/](https://apis.io/providers/ownerrez/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for OwnerRez: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/ownerrez/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
