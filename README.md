# Quaderno (quaderno)

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

Quaderno is a tax compliance, invoicing, and sales-tax / VAT automation platform. Its REST API calculates the correct sales tax, VAT, and GST in real time for any jurisdiction, then issues tax-compliant invoices, credit notes, estimates, and receipts. The account-scoped API (`https://ACCOUNT_NAME.quadernoapp.com/api`) covers contacts, items, invoices, credits, estimates, expenses, recurring documents, payments, unified sales transactions, hosted Checkout sessions, and webhooks, plus a tax engine for rate calculation, jurisdictions, tax codes, and tax ID validation. Requests use HTTP Basic Auth with a private API key and return JSON; every endpoint path ends in `.json`.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/quaderno/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/quaderno/refs/heads/main/apis.yml)

## Tags

- Tax Compliance
- Sales Tax
- VAT
- Invoicing
- Billing
- FinTech

## Timestamps

- **Created:** 2026-07-03
- **Modified:** 2026-07-03

## APIs

### Quaderno Invoices API

Create, list, retrieve, update, delete, and deliver tax-compliant sales invoices, each with line items, taxes, discounts, currency, and a public permalink. Invoices carry nested payments and can be emailed to the contact.

- **Human URL:** [https://developers.quaderno.io/api/](https://developers.quaderno.io/api/)
- **Base URL:** `https://ACCOUNT_NAME.quadernoapp.com/api`

### Quaderno Credits API

Issue and manage credit notes against invoices - create, list, retrieve, update, and delete credits with their own line items, taxes, and totals for refunds and corrections.

- **Human URL:** [https://developers.quaderno.io/api/](https://developers.quaderno.io/api/)
- **Base URL:** `https://ACCOUNT_NAME.quadernoapp.com/api`

### Quaderno Estimates API

Create, list, retrieve, update, and delete estimates and quotes issued to customers, with line items, taxes, and state tracking - convertible into invoices once accepted.

- **Human URL:** [https://developers.quaderno.io/api/](https://developers.quaderno.io/api/)
- **Base URL:** `https://ACCOUNT_NAME.quadernoapp.com/api`

### Quaderno Expenses API

Record and manage vendor bills and purchases - create, list, retrieve, update, and delete expenses with line items, taxes, and payment methods for input-tax tracking and reporting.

- **Human URL:** [https://developers.quaderno.io/api/](https://developers.quaderno.io/api/)
- **Base URL:** `https://ACCOUNT_NAME.quadernoapp.com/api`

### Quaderno Contacts API

Manage customers and vendors - create, list, search, retrieve, update, and delete contacts (companies or people) with billing address, country, email, and tax ID used for tax determination.

- **Human URL:** [https://developers.quaderno.io/api/](https://developers.quaderno.io/api/)
- **Base URL:** `https://ACCOUNT_NAME.quadernoapp.com/api`

### Quaderno Items API

Maintain the catalog of reusable products and services - create, list, retrieve, update, and delete items with unit cost, code, stock, and a tax code that drives taxability on documents.

- **Human URL:** [https://developers.quaderno.io/api/](https://developers.quaderno.io/api/)
- **Base URL:** `https://ACCOUNT_NAME.quadernoapp.com/api`

### Quaderno Taxes API

The tax engine - calculate the correct sales tax, VAT, or GST rate in real time (`tax_rates/calculate`) with a reasoning status of taxable, non_taxable, or not_registered; list the tax jurisdictions you are registered in; list product tax codes; and validate customer tax IDs / VAT numbers.

- **Human URL:** [https://developers.quaderno.io/api/](https://developers.quaderno.io/api/)
- **Base URL:** `https://ACCOUNT_NAME.quadernoapp.com/api`

### Quaderno Payments API

Record and remove payments against invoices, credits, and expenses - add a payment with amount, method, and date to mark a document paid, or delete a payment to reverse it.

- **Human URL:** [https://developers.quaderno.io/api/](https://developers.quaderno.io/api/)
- **Base URL:** `https://ACCOUNT_NAME.quadernoapp.com/api`

### Quaderno Transactions API

Record a sale and calculate its tax in a single call - the transactions endpoint determines tax from customer location evidence and item tax codes and creates the corresponding tax-compliant document.

- **Human URL:** [https://developers.quaderno.io/api/](https://developers.quaderno.io/api/)
- **Base URL:** `https://ACCOUNT_NAME.quadernoapp.com/api`

### Quaderno Checkout API

Create and retrieve hosted Checkout sessions that collect tax-compliant payments - rendered client-side with Quaderno.js or as a hosted page - and surface checkout.succeeded, checkout.failed, and checkout.abandoned events.

- **Human URL:** [https://developers.quaderno.io/guides/checkout/](https://developers.quaderno.io/guides/checkout/)
- **Base URL:** `https://ACCOUNT_NAME.quadernoapp.com/api`

### Quaderno Webhooks API

Subscribe URLs to real-time event notifications delivered as JSON over HTTPS - create, list, retrieve, update, and delete webhooks for document and checkout events, with automatic hourly retries for up to 72 hours on failure.

- **Human URL:** [https://developers.quaderno.io/guides/webhooks/](https://developers.quaderno.io/guides/webhooks/)
- **Base URL:** `https://ACCOUNT_NAME.quadernoapp.com/api`

## Authentication

HTTP Basic Authentication. Use your private API key as the username; any value works for the password. All requests and responses are JSON, and every endpoint path ends in `.json`.

## Rate Limits

100 requests per 15 seconds per account. Exceeding the limit returns HTTP 429 (Too Many Requests). The `/ping` endpoint checks availability and remaining allowance without consuming rate limit. See [rate-limits/quaderno-rate-limits.yml](rate-limits/quaderno-rate-limits.yml).

## Common Properties

- [GitHub Organization](https://github.com/quaderno)
- [LinkedIn](https://www.linkedin.com/company/quaderno)
- [Website](https://quaderno.io)
- [Documentation](https://developers.quaderno.io)
- [Plans](plans/quaderno-plans-pricing.yml)
- [Rate Limits](rate-limits/quaderno-rate-limits.yml)
- [Fin Ops](finops/quaderno-finops.yml)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
