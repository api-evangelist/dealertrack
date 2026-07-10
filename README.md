# Dealertrack (dealertrack)

Dealertrack is a [Cox Automotive](https://www.coxautoinc.com/brands/dealertrack/) brand providing automotive dealership software - a cloud-based Dealer Management System (DMS), digital contracting and F&I tools, and the largest dealer-to-lender credit application network in the United States.

**Access model: partner-gated.** Dealertrack does **not** publish an open, self-service public API. Its developer surface is reached two ways, both of which require onboarding:

- **Opentrack** - the Dealertrack DMS third-party integration program. Described as secure, real-time, and bidirectional, it lets certified vendors pull DMS data (vehicles, customers, deals, repair orders, parts, general ledger) and push data back (new deals, customer updates, service appointments, payments, journal entries). A vendor must complete Opentrack certification and pay nominal annual fees plus per-vendor/per-API data-access fees, or integrate through an already-certified Opentrack partner. Access is authorized per dealer by dealership administrators. The DMS platform advertises 375+ OEM integration points and 275+ certified third-party vendors.
- **Cox Automotive Integration Platform** ([developer.coxautoinc.com](https://developer.coxautoinc.com/)) - the OAuth-secured (Okta) partner storefront through which Cox Automotive brand APIs, including Dealertrack credit/F&I functions, are exposed to onboarded partners.

No open API reference, self-service signup, public base URL, SDK, or public WebSocket/SSE endpoint was found. The APIs in this entry are documented honestly with an `endpointsModeled` flag - the operations are inferred from public product and program documentation, not copied from an open API reference, and no endpoints have been fabricated.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/dealertrack/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/dealertrack/refs/heads/main/apis.yml)

## Divestiture note

Dealertrack's Registration & Titling businesses - RTS (Registration and Titling Solutions), RegUSA (nationwide title and registration), Accelerated Title, and CMS (Collateral Management Services) - were divested by Cox Automotive to **Vitu** (acquisition closed January 2025). Those registration/titling capabilities are therefore **not** modeled here as Dealertrack APIs.

## Tags

- Automotive
- Dealership
- DMS
- F&I
- Credit Application
- Lender Network
- Cox Automotive
- Opentrack
- Partner Gated

## Timestamps

- **Created:** 2026-07-10
- **Modified:** 2026-07-10

## APIs (modeled, partner-gated)

### Dealertrack Opentrack DMS Data API

Real-time, bidirectional **read** access to Dealertrack DMS data through the Opentrack integration program - vehicle inventory, customers, deals, repair orders, parts, and general ledger / accounting. Partner-gated; endpoints modeled from program documentation.

- **Program:** [Opentrack integration](https://us.dealertrack.com/resources/dealertrack-dms-opentrack-integration/)
- **Portal:** [developer.coxautoinc.com](https://developer.coxautoinc.com/)

### Dealertrack Opentrack DMS Write-Back API

Real-time, bidirectional **write** access to the DMS through Opentrack - creating new deals, updating customer records, booking service appointments, posting payments, and writing journal entries. Partner-gated; endpoints modeled.

- **Program:** [Opentrack integration](https://us.dealertrack.com/resources/dealertrack-dms-opentrack-integration/)
- **Portal:** [developer.coxautoinc.com](https://developer.coxautoinc.com/)

### Dealertrack Credit and Lender Network API

Programmatic access to Dealertrack's dealer-to-lender credit application network and F&I / eContracting workflow, exposed to certified partners through the Cox Automotive Integration Platform under an OAuth-secured partner model. Partner-gated; endpoints modeled.

- **Portal:** [developer.coxautoinc.com](https://developer.coxautoinc.com/)

## Common Properties

- [LinkedIn](https://www.linkedin.com/company/dealertrack)
- [Website](https://us.dealertrack.com/)
- [Documentation / Portal](https://developer.coxautoinc.com/)
- [Plans](plans/dealertrack-plans-pricing.yml)
- [Rate Limits](rate-limits/dealertrack-rate-limits.yml)
- [Fin Ops](finops/dealertrack-finops.yml)

## WebSocket Review

**Does Dealertrack expose a documented public WebSocket API?** No. See [review.yml](review.yml). All integration surfaces are partner-gated request/response REST over HTTPS; no public WebSocket (ws:// or wss://) or server-push transport is documented, so no AsyncAPI document was authored.

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
