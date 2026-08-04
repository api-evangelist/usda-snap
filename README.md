# USDA SNAP Retailer Locator (usda-snap)

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
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

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
