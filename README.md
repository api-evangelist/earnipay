# Earnipay

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

Earnipay is a Nigerian fintech that operates an NRS/FIRS-compliant e-invoicing platform for businesses. As an accredited Nigeria Revenue Service (NRS) and NITDA systems integrator, Earnipay lets developers programmatically create businesses, manage customers and products, generate FIRS-compliant invoices with IRN (Invoice Reference Number) and QR codes, and submit them to the tax authority through an Access Point Provider (APP) connection. The public Earnipay Invoicing API is an OpenAPI 3.0.0 REST service covering authentication, businesses, customers, products, payment details, invoices, IRN and QR generation, bank lookup/verification, and team management. It authenticates with JWT bearer tokens for user-facing flows and an X-API-Key header for third-party integrations. Added to the API Evangelist network as a portfolio company of Canaan Partners.

**Areas:** Company · E-Invoicing · Invoicing · FIRS · NRS · Tax · Compliance · Fintech · Nigeria · Payments · Financial Services

## Earnipay on APIs.io

Everything profiled for Earnipay is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/earnipay/](https://apis.io/providers/earnipay/)** — or go straight to one of the APIs or properties below.

### APIs (13)

- [Earnipay App API](https://apis.io/apis/earnipay/earnipay-app-api/) — The App API from Earnipay — 1 operation(s) for app.
- [Earnipay APP Provider API](https://apis.io/apis/earnipay/earnipay-app-provider-api/) — Third-party APP provider integration (Taxly) for FIRS submission
- [Earnipay Authentication API](https://apis.io/apis/earnipay/earnipay-authentication-api/) — User authentication and authorization endpoints
- [Earnipay Bank API](https://apis.io/apis/earnipay/earnipay-bank-api/) — The Bank API from Earnipay — 2 operation(s) for bank.
- [Earnipay Business API](https://apis.io/apis/earnipay/earnipay-business-api/) — Business profile management and FIRS configuration
- [Earnipay Customers API](https://apis.io/apis/earnipay/earnipay-customers-api/) — Customer management for invoicing
- [Earnipay Invoices API](https://apis.io/apis/earnipay/earnipay-invoices-api/) — Invoice creation, management, and FIRS validation
- [Earnipay IRN Generator API](https://apis.io/apis/earnipay/earnipay-irn-generator-api/) — Generate FIRS-compliant Invoice Reference Numbers
- [Earnipay Payment Details API](https://apis.io/apis/earnipay/earnipay-payment-details-api/) — The Payment Details API from Earnipay — 2 operation(s) for payment details.
- [Earnipay Products API](https://apis.io/apis/earnipay/earnipay-products-api/) — The Products API from Earnipay — 2 operation(s) for products.
- [Earnipay QR Code Generator API](https://apis.io/apis/earnipay/earnipay-qr-code-generator-api/) — Generate FIRS-compliant encrypted QR codes for invoices
- [Earnipay Team API](https://apis.io/apis/earnipay/earnipay-team-api/) — Team member and invitation management
- [Earnipay Users API](https://apis.io/apis/earnipay/earnipay-users-api/) — User profile management

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### MCP servers (1)

Model Context Protocol servers that expose the API to agents.

- [earnipay-invoicing](https://apis.io/servers/earnipay/earnipay-invoicing/)

#### Agentic access (1)

Which operations an agent can call, which act, and which need a human in the loop.

- [Earnipay Agentic Access](https://apis.io/agentic-access/earnipay/earnipay-agentic-access/)

#### Collections (13)

Postman and Open Collection request collections.

- [Earnipay Invoicing App API](https://apis.io/collections/earnipay/open-earnipay-app-api/)
- [Earnipay Invoicing App APP Provider API](https://apis.io/collections/earnipay/open-earnipay-app-provider-api/)
- [Earnipay Invoicing App Authentication API](https://apis.io/collections/earnipay/open-earnipay-authentication-api/)
- [Earnipay Invoicing App Bank API](https://apis.io/collections/earnipay/open-earnipay-bank-api/)
- [Earnipay Invoicing App Business API](https://apis.io/collections/earnipay/open-earnipay-business-api/)
- [Earnipay Invoicing App Customers API](https://apis.io/collections/earnipay/open-earnipay-customers-api/)
- [Earnipay Invoicing App Invoices API](https://apis.io/collections/earnipay/open-earnipay-invoices-api/)
- [Earnipay Invoicing App IRN Generator API](https://apis.io/collections/earnipay/open-earnipay-irn-generator-api/)
- [Earnipay Invoicing App Payment Details API](https://apis.io/collections/earnipay/open-earnipay-payment-details-api/)
- [Earnipay Invoicing App Products API](https://apis.io/collections/earnipay/open-earnipay-products-api/)
- [Earnipay Invoicing App QR Code Generator API](https://apis.io/collections/earnipay/open-earnipay-qr-code-generator-api/)
- [Earnipay Invoicing App Team API](https://apis.io/collections/earnipay/open-earnipay-team-api/)
- [Earnipay Invoicing App Users API](https://apis.io/collections/earnipay/open-earnipay-users-api/)

#### Overlays (1)

OpenAPI overlays, including conversational phrasing for each operation.

- [Earnipay E Invoicing Overlay](https://apis.io/overlays/earnipay/earnipay-e-invoicing-overlay/)

#### Security (2)

Authentication, trust centre, and vulnerability disclosure.

- [Earnipay Authentication](https://apis.io/security/earnipay/earnipay-authentication/)
- [Earnipay Domain Security](https://apis.io/security/earnipay/earnipay-domain-security/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://earnipay.com/)
- [Documentation](https://docs.earnipay.com/docs/e-invoice)
- [Getting started](https://docs.earnipay.com/docs/e-invoice)
- [API reference](https://e-invoicing.earnipay.com/api/docs)
- [Blog](https://www.earnipay.com/blog/)
- [GitHub](https://github.com/Earnipay)

## API Evangelist rating

**Kin Score 22.6** — emerging · rubric 0.24.0 · scored 2026-10-17

| Facet | Score |
|---|---|
| Discoverability | 73.2 |
| Contract quality | 44.3 |
| Contract governance | 4.5 |
| Operational transparency | 2.6 |
| Developer ergonomics | 23.2 |
| Access clarity | 0.0 |

**Agent readiness 25.7** — agent-aware

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | yes |
| Agentic Access | derived (partial credit) |
| Reversibility Documented | verified |
| MCP Server | — |
| Auth Clarity | bearer (partial credit) |
| Idempotency | — |
| Error Semantics | derived (partial credit) |
| OpenAPI Examples | partial |
| Rate Limit Signal | — |
| Event Surface Described | — |
| Agent Skills | derived (partial credit) |
| Well Known Catalog | — |
| Consent Identity | — |
| Agent Card | — |
| Dry Run Mode | — |
| Delegated Identity | — |
| Protected Resource Metadata | — |
| Dynamic Client Registration | — |
| Agentic Commerce | — |

**Regulatory alignment 15.2** — Payments

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/earnipay/](https://apis.io/providers/earnipay/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for Earnipay: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/earnipay/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
