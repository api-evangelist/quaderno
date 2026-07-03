# Quaderno (quaderno)

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
