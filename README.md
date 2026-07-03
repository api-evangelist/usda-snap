# USDA SNAP Retailer Locator (usda-snap)

The USDA Food and Nutrition Administration (FNA) - renamed from the Food and Nutrition Service (FNS) on June 1, 2026 - publishes an open, public geospatial API for the Supplemental Nutrition Assistance Program (SNAP) Retailer Locator. The data is hosted as an Esri ArcGIS Feature Service (`snap_retailer_location_data`) rather than a bespoke `fns.usda.gov` or `api.fns.usda.gov` endpoint, and is embedded directly in the public retailer locator tool at [fna.usda.gov/snap/retailer-locator](https://www.fna.usda.gov/snap/retailer-locator). It exposes point-in-time location records - name, address, city, state, zip, county, store type, latitude/longitude, and Healthy Incentive Program participation - for every currently authorized SNAP retailer nationwide (254,048 records confirmed live on the review date), queryable anonymously over REST with no API key, in JSON, GeoJSON, or PBF, with CSV/Shapefile/KML export also available through the ArcGIS Hub item page. The service is read-only (Query only - no write capabilities).

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/usda-snap/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/usda-snap/refs/heads/main/apis.yml)

## Tags

- SNAP
- USDA
- Food and Nutrition Administration
- FNA
- FNS
- Retailer Locator
- Open Data
- ArcGIS
- GIS
- Government Data
- Food Assistance

## Timestamps

- **Created:** 2026-07-03
- **Modified:** 2026-07-03

## APIs

### SNAP Retailer Location Data API

Public, anonymous, read-only Esri ArcGIS Feature Service exposing location records for every currently authorized SNAP retailer nationwide - store name, street address, city, state, zip/zip4, county, store type (e.g. Convenience Store, Grocery Store, Supermarket, Super Store, Farmers and Markets, Restaurant Meals Program, Specialty Store, Other), latitude and longitude, and Healthy Incentive Program / grantee participation. Supports SQL-style `where` filtering, field selection, spatial queries, sorting, distinct values, statistics, and offset-based pagination (maxRecordCount 1,000 rows per request) in JSON, GeoJSON, or PBF. This is the same live data source (ArcGIS item `8b260f9a10b0459aa441ad8588c2251c`) embedded in FNA's own public retailer locator web tool.

- **Human URL:** [https://www.fna.usda.gov/snap/retailer-locator](https://www.fna.usda.gov/snap/retailer-locator)
- **Base URL:** `https://services1.arcgis.com/RLQu0rK7h4kbsBq5/arcgis/rest/services/snap_retailer_location_data/FeatureServer`

#### Tags

- Retailers
- Locations
- Geospatial
- ArcGIS Feature Service
- Open Data

#### Properties

- [Website](https://www.fna.usda.gov/snap/retailer-locator)
- [Documentation](https://developers.arcgis.com/rest/services-reference/enterprise/query-feature-service-layer/)
- [API Reference](https://www.arcgis.com/home/item.html?id=8b260f9a10b0459aa441ad8588c2251c)
- [Documentation](https://usda-snap-retailers-usda-fns.hub.arcgis.com/datasets/USDA-FNS::snap-retailer-location-data/)
- [OpenAPI](openapi/usda-snap-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/usda-snap.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/usda-snap.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [Website](https://www.fna.usda.gov/snap/retailer-locator)
- [Documentation](https://developers.arcgis.com/rest/services-reference/enterprise/query-feature-service-layer/)
- [Rate Limits](rate-limits/usda-snap-rate-limits.yml)
- [Review](review.yml)

## Plans and FinOps

Not applicable. This is free, public U.S. government open data with no pricing tiers, billing, or cost dimension - `plans/` and `finops/` are intentionally omitted rather than fabricated.

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
