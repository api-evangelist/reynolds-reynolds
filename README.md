# Reynolds and Reynolds (reynolds-reynolds)

Reynolds and Reynolds is one of the automotive industry's largest Dealership Management System (DMS) providers. Its ERA-IGNITE and POWER platforms run the core of thousands of franchised car dealerships - sales and desking, F&I, service and repair orders, parts inventory, CRM, and dealership accounting.

**Important: there is no open, self-serve Reynolds developer API.** Reynolds does not publish a public developer portal, a public API reference, or an OpenAPI definition. All sanctioned programmatic access to a dealer's Reynolds DMS flows through the **Reynolds Certified Interface (RCI)** program, run by Reynolds Data Management.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/reynolds-reynolds/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/reynolds-reynolds/refs/heads/main/apis.yml)

## Access Model: Certification-Gated Partner Program

The Reynolds Certified Interface (RCI) program has provided the industry's controlled path to Reynolds DMS data since 2005. Its defining characteristics:

- **Certification required.** A third party must apply, pass a technical and security review, and be certified before it can integrate. Reynolds maintains a public list of certified RCI third-party vendors.
- **Contract and NDA.** RCI terms, interface specifications, and pricing are covered by NDA and negotiated per partner. They are not published.
- **Secured, real-time, bi-directional.** RCI delivers real-time interfaces that can both read from and write back to a dealer's Reynolds DMS (the "DMS write-back" pattern used by inventory, pricing, service-scheduling, and CRM vendors).
- **Not free, not instant.** Publicly reported figures are anecdotal and dated - a dealer forum cited roughly $70K circa 2007 plus recurring per-dealer ("rooftop") fees, with a multi-month certification queue. Treat these as directional only; contact Reynolds Data Management for current terms.

Because there is no public API specification, the APIs listed here are **logical DMS data domains** exposed through RCI, and their endpoints are **modeled, not sourced** from any public Reynolds documentation. No public base URLs, endpoint paths, or authentication schemes are asserted.

## Tags

- Automotive
- Dealership Management System
- DMS
- Reynolds Certified Interface
- RCI
- Certified Interface
- Partner API
- Gated Access

## Timestamps

- **Created:** 2026-07-10
- **Modified:** 2026-07-10

## APIs (logical domains, endpoints modeled)

### Reynolds DMS Customer Data API

Customer and prospect records held in the Reynolds DMS - contact details, ownership history, and marketing consent - read and (per certification scope) written back through RCI.

- **Documentation:** [Reynolds Certified Interface](https://www.reyrey.com/partners/reynolds-certified-interface)

### Reynolds Vehicle Inventory API

New and used vehicle inventory - VINs, stock numbers, pricing, and status - available to certified partners for read and pricing write-back.

- **Documentation:** [Reynolds Certified Interface](https://www.reyrey.com/partners/reynolds-certified-interface)

### Reynolds Sales, Deals and F&I API

Retail and lease deal, desking, and Finance and Insurance data - deal structures, lender submissions, and F&I products - for certified partners.

- **Documentation:** [Reynolds Certified Interface](https://www.reyrey.com/partners/reynolds-certified-interface)

### Reynolds Service and Repair Orders API

Repair orders, labor operations, and service appointments. Certified scheduling partners push appointments into the DMS and pull DMS appointments and repair orders in real time.

- **Documentation:** [Reynolds Certified Interface](https://www.reyrey.com/partners/reynolds-certified-interface)

### Reynolds Parts Inventory API

Parts on-hand quantities, pricing, purchase orders, and suppliers, for certified parts, catalog, and e-commerce partners.

- **Documentation:** [Reynolds Certified Interface](https://www.reyrey.com/partners/reynolds-certified-interface)

### Reynolds Accounting API

Dealership accounting - general ledger, AR/AP, cash receipts, and postings - exposed to certified accounting and reporting partners.

- **Documentation:** [Reynolds Certified Interface](https://www.reyrey.com/partners/reynolds-certified-interface)

## Common Properties

- [LinkedIn](https://www.linkedin.com/company/reynolds-and-reynolds)
- [Website](https://www.reyrey.com)
- [Documentation - Reynolds Certified Interface](https://www.reyrey.com/partners/reynolds-certified-interface)
- [Sign Up - Reynolds Data Management](https://www.reyrey.com/company/reynolds-data-management)
- [Plans](plans/reynolds-reynolds-plans-pricing.yml)

## WebSocket Review

Does Reynolds and Reynolds expose a documented public WebSocket API? **No.** See [review.yml](review.yml). Reynolds publishes no public API of any kind; all access is gated behind the certification-only, NDA-covered RCI program, and no WebSocket endpoint is documented publicly.

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
