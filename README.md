# ShipBob (shipbob)

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

ShipBob is a Chicago-based global ecommerce fulfillment network and 3PL operating 60+ fulfillment centers, providing distributed warehousing, inventory, B2B/EDI, and shipping operations for direct-to-consumer brands with a developer-friendly REST API.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/shipbob/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/shipbob/refs/heads/main/apis.yml)

## Tags

- Logistics
- Fulfillment
- 3PL
- Ecommerce
- Inventory
- Warehousing
- Shipping
- Direct-to-Consumer

## Timestamps

- **Created:** 2026-05-08
- **Modified:** 2026-05-30

## APIs

### ShipBob Developer API

ShipBob Developer API provides versioned REST endpoints for channels, orders, products, inventory, receiving orders, returns, webhooks, locations, billing, and shipment simulations. Latest API version is 2026-01 (released February 2026); selectable via dated URL prefix (e.g. /2026-01/order). Authentication via Personal Access Token (PAT) for single-user integrations or OAuth 2.0 for multi-tenant App Store apps. Sliding-window rate limit of 150 requests/minute per user per application; throttled responses return HTTP 429 with `x-retry-after` and `x-remaining-calls` headers.

- **Human URL:** [https://developer.shipbob.com/](https://developer.shipbob.com/)
- **Base URL:** `https://api.shipbob.com`

#### Tags

- Logistics
- Fulfillment
- REST
- 3PL
- Ecommerce
- Inventory
- Webhooks

#### Properties

- [Documentation](https://developer.shipbob.com/)
- [Authentication](https://developer.shipbob.com/auth)
- [Quickstart](https://developer.shipbob.com/quickstart)
- [Release Notes](https://developer.shipbob.com/release-notes)
- [Rate Limit](https://developer.shipbob.com/rate-limit)
- [F A Q](https://developer.shipbob.com/faq)
- [OpenAPI](openapi/shipbob-openapi.json) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/shipbob.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/shipbob.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [AsyncAPI](asyncapi/shipbob-webhooks-asyncapi.yml) — [AsyncAPI Specification](https://www.asyncapi.com/docs/reference/specification/latest)

## Common Properties

- [Website](https://www.shipbob.com/)
- [Documentation](https://developer.shipbob.com/)
- [Pricing](https://www.shipbob.com/pricing/)
- [App Store](https://www.shipbob.com/integrations/)
- [Support Portal](https://support.shipbob.com/)
- [GitHub Organization](https://github.com/ShipBob)
- [LinkedIn](https://www.linkedin.com/company/shipbob)
- [Plans](plans/shipbob-plans-pricing.yml)
- [Rate Limits](rate-limits/shipbob-rate-limits.yml)
- [Fin Ops](finops/shipbob-finops.yml)
- [L L Ms Txt](https://developer.shipbob.com/llms.txt)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
