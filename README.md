# ShipBob (shipbob)

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
