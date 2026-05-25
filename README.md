# ShipBob (shipbob)

ShipBob is a Chicago-based global ecommerce fulfillment network and 3PL operating 60+ fulfillment centers, providing distributed warehousing, inventory, B2B/EDI, and shipping operations for direct-to-consumer brands with a developer-friendly REST API.

**URL:** [Visit APIs.json URL](https://raw.githubusercontent.com/api-evangelist/shipbob/refs/heads/main/apis.yml)

**Run:** [Capabilities Using Naftiko](https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=shipbob-api-evangelist&utm_content=repo)

## Tags

- Logistics, Fulfillment, 3PL, Ecommerce, Inventory, Warehousing, Shipping, Direct-to-Consumer

## Timestamps

- **Created:** 2026-05-08
- **Modified:** 2026-05-25

## APIs

### ShipBob Developer API

ShipBob Developer API provides versioned REST endpoints for channels, orders, products, inventory, receiving orders, returns, webhooks, locations, billing, and shipment simulations. Latest API version is 2026-01 (released February 2026); selectable via dated URL prefix (e.g. `/2026-01/order`). Authentication via Personal Access Token (PAT) for single-user integrations or OAuth 2.0 for multi-tenant App Store apps. Sliding-window rate limit of 150 requests/minute per user per application; throttled responses return HTTP 429 with `x-retry-after` and `x-remaining-calls` headers.

**Human URL:** [https://developer.shipbob.com/](https://developer.shipbob.com/)

**Base URL:** `https://api.shipbob.com`

#### Tags

- Logistics, Fulfillment, REST, 3PL, Ecommerce, Inventory, Webhooks

#### Properties

- [Documentation](https://developer.shipbob.com/)
- [Authentication](https://developer.shipbob.com/auth)
- [Quickstart](https://developer.shipbob.com/quickstart)
- [ReleaseNotes](https://developer.shipbob.com/release-notes)
- [RateLimit](https://developer.shipbob.com/rate-limit)
- [FAQ](https://developer.shipbob.com/faq)
- [OpenAPI](openapi/shipbob-openapi.json)

## Common Properties

- [Website](https://www.shipbob.com/)
- [Documentation](https://developer.shipbob.com/)
- [Pricing](https://www.shipbob.com/pricing/)
- [AppStore](https://www.shipbob.com/integrations/)
- [SupportPortal](https://support.shipbob.com/)
- [GitHubOrganization](https://github.com/ShipBob)
- [LinkedIn](https://www.linkedin.com/company/shipbob)
- [Plans](plans/shipbob-plans-pricing.yml)
- [RateLimits](rate-limits/shipbob-rate-limits.yml)
- [FinOps](finops/shipbob-finops.yml)
- [LLMsTxt](https://developer.shipbob.com/llms.txt)

## Artifacts

Machine-readable API specifications organized by format.

### OpenAPI

- [ShipBob Developer API](openapi/shipbob-openapi.json)

## Capabilities

Naftiko capabilities organized per ShipBob business surface. Each file is a self-contained workflow capability with REST and MCP exposers.

| Capability | Tools | Surface |
|------------|-------|---------|
| [Billing](capabilities/shipbob-subpackage-billing.yaml) | 8 | Invoices and billing events |
| [Channels](capabilities/shipbob-subpackage-channels.yaml) | 2 | Sales channel inventory |
| [Inventory](capabilities/shipbob-subpackage-inventory.yaml) | 18 | Inventory levels and history |
| [Locations](capabilities/shipbob-subpackage-locations.yaml) | 2 | Fulfillment center directory |
| [Orders](capabilities/shipbob-subpackage-orders.yaml) | 43 | Order lifecycle and shipments |
| [Products](capabilities/shipbob-subpackage-products.yaml) | 27 | Catalog and SKUs |
| [Receiving](capabilities/shipbob-subpackage-receiving.yaml) | 17 | Warehouse Receiving Orders |
| [Returns](capabilities/shipbob-subpackage-returns.yaml) | 8 | Return management |
| [Simulations](capabilities/shipbob-subpackage-simulations.yaml) | 4 | Sandbox shipment simulations |
| [Webhooks](capabilities/shipbob-subpackage-webhooks.yaml) | 5 | Subscription management |

## Plans, Rate Limits, and FinOps

- [Plans](plans/shipbob-plans-pricing.yml) — Quote-based fulfillment account with documented $275/month minimum; per-unit pick-and-pack, storage, receiving, and shipping fees. API access is included.
- [Rate Limits](rate-limits/shipbob-rate-limits.yml) — 150 requests/minute sliding window per user, per application; 429 with `x-retry-after` and `x-remaining-calls` headers.
- [FinOps](finops/shipbob-finops.yml) — FOCUS-aligned view of ShipBob's quote-based 3PL billing model.

## References

- Reviewed and profiled with assistance from [Anthropic](https://www.anthropic.com/) Claude via Claude Code.

## Maintainers

**FN:** Kin Lane

**Email:** kin@apievangelist.com
