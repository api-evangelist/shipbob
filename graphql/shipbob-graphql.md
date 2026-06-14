# ShipBob GraphQL Schema

## Overview

ShipBob is a global ecommerce fulfillment network and third-party logistics (3PL) provider operating 60+ fulfillment centers. This conceptual GraphQL schema models the core domain objects surfaced by the ShipBob Developer REST API, covering orders, inventory, products, shipments, returns, receiving, channels, locations, and account management.

ShipBob's public API is REST-based (https://developer.shipbob.com/), with versioned endpoints selectable via dated URL prefixes (e.g. `/2026-01/order`). This GraphQL schema translates those REST resources into a unified type system suitable for wrapping with a GraphQL gateway or for documentation and tooling purposes.

## Authentication

ShipBob supports two authentication mechanisms:

- **Personal Access Token (PAT):** Single-user integrations; token passed in the `Authorization: Bearer <token>` header.
- **OAuth 2.0:** Multi-tenant App Store apps; standard authorization code flow with scopes per resource domain.

Rate limit: 150 requests per minute per user per application (sliding window). Throttled responses include `x-retry-after` and `x-remaining-calls` headers.

## Schema Source

- API Docs: https://developer.shipbob.com/
- GitHub: https://github.com/ShipBob
- Schema file: `shipbob-schema.graphql`

## Core Type Domains

### Orders

Covers the full lifecycle of a merchant order from creation through fulfillment. Key types: `Order`, `OrderDetails`, `OrderStatus`, `OrderHistory`, `OrderProduct`, `OrderItem`, `OrderAddress`, `ShipTo`, `Recipient`, `ReturnAddress`, `OrderMetadata`, `CustomFields`, `OrderQuantities`.

### Locations & Warehouses

Models ShipBob's distributed fulfillment network. Key types: `Location`, `Warehouse`, `WarehouseDetails`, `WarehouseCapacity`, `FulfillmentCenter`.

### Inventory

Tracks stock levels across fulfillment centers. Key types: `Inventory`, `InventoryItem`, `InventoryQuantity`, `InventoryLocation`, `InventoryLog`.

### Products

Represents merchant catalog items. Key types: `Product`, `ProductDetails`, `ProductSKU`, `ProductBarcode`, `ProductWeight`, `ProductDimension`, `BundleProduct`, `BundleParts`.

### Shipments

Models outbound shipment events and packages. Key types: `Shipment`, `ShipmentDetails`, `ShipmentStatus`, `ShipmentPackages`, `Package`, `PackageDetail`, `PackageWeight`, `PackageDimension`, `Parcel`, `Label`, `TrackingInfo`, `TrackingEvent`, `TrackingStatus`.

### Returns

Covers return merchandise authorization (RMA) and return inventory disposition. Key types: `Return`, `ReturnDetails`, `ReturnStatus`, `ReturnInventory`.

### Receiving

Models inbound purchase orders and warehouse receiving workflows. Key types: `Receiving`, `ReceivingDetails`.

### Channels & Account

Covers sales channel mappings and account/API credential management. Key types: `Channel`, `ChannelMapping`, `User`, `Account`, `APIKey`, `Token`, `Webhook`.

## Query Capabilities

- Fetch single orders, shipments, products, or inventory items by ID
- List and filter orders by status, channel, date range, and location
- Retrieve inventory levels per SKU across all or specific fulfillment centers
- Query shipment tracking history and package details
- List returns and receiving orders with status filters
- Manage webhooks and channel configurations

## Mutation Capabilities

- Create and cancel orders
- Create products and update product details
- Create receiving (inbound) orders
- Create and update return records
- Register and delete webhooks
- Manage channel mappings
