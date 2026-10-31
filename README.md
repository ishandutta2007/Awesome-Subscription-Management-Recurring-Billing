# Awesome-Subscription-Management-Recurring-Billing

# Top Subscription Management & Recurring Billing Ecosystem

**Curated List of SaaS Products & Open-Source GitHub Projects**  
*Focused on Subscription Lifecycle Automation, Usage Metering & Self-Hosted Billing Engines*  
**Last updated: October 2026**

This repository tracks notable **SaaS platforms** and **open-source projects** for **Subscription Management & Recurring Billing**. These tools enable businesses to manage recurring revenue—handling plan catalogs, subscription lifecycle events (create, upgrade, pause, cancel), usage-based metering, invoicing, dunning, and tax—turning complex billing logic into a controlled, auditable system.

**Examples** include HubSpot Subscriptions, Stripe Billing, Chargebee, Zuora, Recurly, Maxio, Paddle, FastSpring, Rebilly, and Ordway (the category leaders).

**Open-source emphasis**: Subscription Management & Recurring Billing is a domain where open-source tooling is **mature and production-proven for core billing workflows**. **Kill Bill** is the longest-standing open-source billing platform—in production since 2010, Apache 2.0 licensed, with catalog and pricing, subscriptions, usage billing, invoicing, payments via gateway plugins, retries and dunning, tax plugins, multi-tenancy, and audit logs . **Lago** is the strongest open-source alternative for **usage-based billing**—positioned explicitly against Chargebee, Recurly, and Stripe Billing for complex billing logic, with real-time event ingestion, billable metrics aggregation, and automated invoicing . **UniBee** offers a lighter, AGPLv3-licensed SaaS billing alternative with subscriptions, invoices, discounts, and a user portal . The critical caveat: **self-hosting means owning upgrades, payment gateway integrations, tax configuration, and financial data security**—the license is free, but operational responsibility is not .

Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.

## Table of Contents
- [SaaS/Hosted Platforms](#saas-products)
- [Open-Source GitHub Projects](#open-source-github-projects)
- [How to Contribute](#how-to-contribute)
- [Disclaimer](#disclaimer)

## SaaS/Hosted Platforms

- **[HubSpot Subscriptions](https://www.hubspot.com/)**  
  Subscription billing within HubSpot's Commerce Hub; connects recurring payments to CRM records for unified customer and revenue visibility.

- **[Stripe Billing](https://stripe.com/billing)**  
  The developer-standard for recurring billing; handles subscriptions, invoicing, proration, usage-based billing, and dunning with deep integration into Stripe's payment ecosystem.

- **[Chargebee](https://www.chargebee.com/)**  
  Subscription management platform with revenue recognition (Chargebee RevRec), supporting complex billing models, dunning, and integrations with major payment gateways.

- **[Zuora](https://www.zuora.com/)**  
  Enterprise subscription management and revenue recognition platform for recurring revenue businesses; covers billing, collections, and RevPro compliance.

- **[Recurly](https://recurly.com/)**  
  Subscription management and billing platform focused on reducing churn and automating recurring billing workflows.

- **[Maxio](https://www.maxio.com/)**  
  Financial operations platform for B2B SaaS combining subscription billing (Chargify) and revenue recognition (SaaSOptics).

- **[Paddle](https://www.paddle.com/)**  
  Merchant of record for SaaS and digital products; handles global sales tax, VAT, subscription billing, and compliance alongside billing.

- **[FastSpring](https://fastspring.com/)**  
  Merchant of record and ecommerce platform for software and SaaS; handles global tax, payments, subscriptions, and compliance.

- **[Rebilly](https://www.rebilly.com/)**  
  Subscription and recurring billing platform with payment orchestration, dunning, and revenue optimization features.

- **[Ordway](https://ordwaylabs.com/)**  
  Billing and revenue automation platform for subscription businesses; handles complex pricing, invoicing, and revenue recognition.

## Open-Source GitHub Projects

### Full Billing Platforms (Subscriptions + Payments + Invoicing)

- **[Kill Bill](https://github.com/killbill/killbill)**  
  The most mature open-source **subscription billing and payments platform** available (Apache 2.0, in production since 2010)  . Features: **catalog and pricing** (plans, phases, trials, add-ons, multiple currencies), **subscriptions** (create, change, pause, resume, cancel with proration), **usage billing** (tiers or blocks, billed in arrears), **invoicing** (event-driven, generated as events happen), **payments** via gateway plugins (Stripe, Adyen, Braintree, Hyperswitch), **retries and dunning**, **tax** via plugins (Avalara, Vertex, Kintsugi), **multi-tenancy**, **audit logs** (every change recorded), and **tags/custom fields** on any object  . Runs on Docker, Tomcat, or Kubernetes with MySQL/MariaDB/PostgreSQL. Admin UI via **Kaui** (open source). **The strongest open-source foundation for a complete subscription business**—but deployment requires Java expertise and ongoing operational ownership  .

- **[Lago](https://github.com/getlago/lago)**  
  The leading open-source **usage-based billing** platform (AGPL-3.0, founded 2021)  . Positioned explicitly as an alternative to Chargebee, Recurly, and Stripe Billing for **complex billing logic**  . Features: **usage ingestion** at scale with deduplication, **billable metrics** (COUNT, COUNT_UNIQUE, LATEST, MAX, SUM, WEIGHTED SUM), **pricing and packaging** (subscription-based, usage-based, or hybrid), **automated invoicing** (subscription fees at start/end of period, usage charges at period end), and **payment provider integrations** via invoice payload or native connectors  . Self-hosted or Lago Cloud; open-source version is AGPL-3.0 with Premium features under commercial pricing  . **Best for SaaS and API businesses with usage-based or hybrid pricing**—stronger on metering than Kill Bill's core, but newer and with commercial feature gates.

- **[UniBee](https://github.com/UniBee-Billing/unibee)**  
  Open-source **SaaS billing software** (AGPLv3) positioned as an alternative to Recurly, Chargebee, and Paddle  . Features: subscription management (create, update, cancel), invoicing, billable metrics, product/plan management, webhooks, user management, reports, transaction management, discounts, and a user portal . Docker Compose deployment (`docker-compose up`) with database, Redis, and API containers. **Best for SaaS businesses wanting a lighter open-source billing alternative**—smaller community and feature set than Kill Bill or Lago, but simpler to deploy and understand  .

### Additional Strong Open-Source Options

- **BillCycle** — Subscription and usage-based billing engine (Python/FastAPI, PostgreSQL, Celery Beat) with state machine and event sourcing patterns . **Early-stage**—technical implementation is "pending in next iteration" per the PyPI release  . Listed for reference only; not production-ready.
- **stapel-billing** — Django app for credit wallets with immutable transaction ledger, one-off credit packages, recurring subscription plans, Stripe-backed checkout, and idempotent webhooks (MIT)  . **Framework-specific**—best for Django monoliths wanting billing primitives without a full platform.
- **jizhang / Calends / PayLoop** — Self-hosted **personal subscription trackers** (not business billing platforms) for tracking recurring expenses, renewal reminders, and spending analytics  . **Different use case**—these track what you pay, not what you charge customers. Included to distinguish personal expense tracking from business subscription billing.

**Frameworks for building custom systems**: For a **complete subscription business** (catalog → subscription → invoice → payment → dunning → tax), Kill Bill provides the most mature and feature-complete foundation  . For **usage-based or hybrid pricing** with complex metering, Lago is the strongest open-source alternative to Chargebee/Stripe Billing  . For a **lighter SaaS billing platform** with subscriptions and invoices, UniBee offers a simpler deployment path  . For **Django applications needing credit wallets**, stapel-billing provides billing primitives  . No open-source project matches the managed compliance and payment gateway breadth of Stripe Billing or Chargebee—self-hosting means owning integrations and financial data security.

## How to Contribute

1. Fork the repo.
2. Add/edit entries in `README.md` (follow existing format).
3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.
4. Submit PR with a short explanation.

Star the repo if you find it useful!

## Disclaimer

- This is a **community-curated** list — not exhaustive and not an endorsement.
- Subscription billing platforms handling payment card data and financial records must comply with **PCI DSS** requirements and applicable tax regulations (VAT/GST/sales tax); **self-hosted solutions place full responsibility for payment gateway security, tax configuration, and financial data integrity on the operator**  .
- **Open-source subscription billing is mature for core workflows**—Kill Bill provides a complete platform in production since 2010  , and Lago leads on usage-based metering  . However, **no open-source project matches the managed simplicity and gateway breadth of Stripe Billing or Chargebee**; self-hosting requires engineering investment in integrations, upgrades, and compliance. Organizations without billing infrastructure expertise should evaluate commercial platforms.
- Verify license terms for commercial use; Kill Bill uses Apache 2.0  , Lago uses AGPL-3.0 for its open-source core with Premium features under commercial licensing  , and UniBee uses AGPLv3  .

---

**Made for billing engineers, SaaS finance teams, and organizations choosing their subscription infrastructure.**  
Let's make subscription billing more open, but with clear eyes about the payment gateway integrations and compliance responsibilities that self-hosting requires.
