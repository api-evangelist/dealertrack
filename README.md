# Dealertrack (dealertrack)

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
