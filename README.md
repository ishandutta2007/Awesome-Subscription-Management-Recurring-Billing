# Awesome Subscription Management & Recurring Billing

[![Awesome](https://awesome.re/badge.svg)](https://awesome.re)
[![Track Awesome List](https://www.trackawesomelist.com/badge.svg)](https://www.trackawesomelist.com/ishandutta2007/Awesome-Subscription-Management-Recurring-Billing/)
[![GitHub stars](https://img.shields.io/github/stars/ishandutta2007/Awesome-Subscription-Management-Recurring-Billing?style=social)](https://github.com/ishandutta2007/Awesome-Subscription-Management-Recurring-Billing/stargazers)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

> A curated directory of leading SaaS platforms, Merchant of Record (MoR) solutions, open-source billing engines, and usage-based metering tools for subscription management and recurring billing automation.

---

## Sector Overview & Market Dynamics

The global **subscription management and recurring billing market** is valued at approximately **$8.0B to $9.2B** and is projected to expand to **$20B–$30B** over the next decade (growing at a 10.5%–16% CAGR), accelerated by the rapid rise of consumption-based, hybrid, and AI billing models alongside stricter global automated renewal laws and e-invoicing compliance mandates.

From a structural perspective, the sector is **moderately concentrated at the high-end enterprise tier**—dominated by mega-platforms and financial infrastructure titans like Stripe, Zuora, and HubSpot that leverage deep ERP/CRM ecosystem integrations—yet **highly fragmented across the mid-market and SMB long tail**, where specialized Merchants of Record (MoRs), developer-first billing engines, and open-source self-hosted solutions thrive to meet bespoke monetization and regional payment requirements.

---

## Table of Contents

- [Sector Overview & Market Dynamics](#sector-overview--market-dynamics)
- [SaaS & Hosted Billing Platforms](#saas--hosted-billing-platforms)
- [Open-Source GitHub Projects](#open-source-github-projects)
  - [Full Billing Platforms & Metering Engines](#full-billing-platforms--metering-engines)
  - [Payment Switching & Developer Primitives](#payment-switching--developer-primitives)
  - [Personal Subscription Trackers](#personal-subscription-trackers)
- [Choosing the Right Billing Stack](#choosing-the-right-billing-stack)
- [How to Contribute](#how-to-contribute)
- [Disclaimer](#disclaimer)

---

## SaaS & Hosted Billing Platforms

The table below compares top-tier commercial subscription management systems, hosted billing platforms, and Merchants of Record (MoR), sorted in descending order by company scale (market valuation / enterprise capitalization):

| Platform | Company Valuation / Revenue | Starting Pricing Tier | Free Tier / Free Trial Limits | Key Specialization & Core Capabilities |
| :--- | :--- | :--- | :--- | :--- |
| **[Stripe Billing](https://stripe.com/billing)** | ~$159B Valuation (~$6.8B net revenue) | **0.7%** of billing volume (stacked on standard payment gateway processing of 2.9% + $0.30/txn) | **Indefinite free sandbox / test mode** with full API functionality and free customer trials; live mode has $0/mo base platform subscription fee | Developer-standard recurring billing, automated proration, usage-based metering, and smart retries with native gateway connectivity. |
| **[HubSpot Subscriptions](https://www.hubspot.com/)** | ~$13B Market Cap (HUBS, ~$2.6B+ revenue) | **$0/mo** platform base fee on Free Tools (or $95/mo for Professional Hub) + **2.9% + 0.5%** card processing / 0.75% Stripe platform routing | **Free forever plan** with basic recurring invoices, quotes, and payment links; paid tiers offer a **14-day free trial** | Native subscription billing connected directly into HubSpot CRM and Revenue Hub to align marketing, deals, and renewal tracking. |
| **[Chargebee](https://www.chargebee.com/)** | $3.5B Valuation (~$200M+ ARR) | **Starter plan:** $0/mo up to threshold, then 0.75% overage fee (or Performance tier starting from $599/mo) | **Free tier up to $250,000 in cumulative lifetime billing**; includes up to 50,000 API calls/month and basic recurring billing workflows | Subscription lifecycle automation, catalog management, dunning workflows, and ASC 606 revenue recognition across 30+ gateways. |
| **[Zuora](https://www.zuora.com/)** | $1.7B Valuation (~$450M revenue; acquired by Silver Lake) | Enterprise custom quote-based contracts (typically starting from **~$75,000/year**) | **No self-serve free trial**; access is granted via enterprise sales demo sandboxes and guided proof-of-concept evaluations | Enterprise-grade quote-to-revenue automation, multi-entity subscription architecture, complex billing hierarchies, and RevPro compliance. |
| **[Paddle](https://www.paddle.com/)** | $1.4B Valuation (~$85M revenue) | **5% + $0.50** per checkout transaction; $0 monthly platform subscription fee | **Full sandbox testing environment free forever**; $0 upfront software cost (fees only apply to completed live sales transactions) | Merchant of Record (MoR) for software and SaaS; automatically handles global VAT/sales tax liabilities, payment routing, and dunning. |
| **[Recurly](https://recurly.com/)** | PE-backed (Accel-KKR, ~$100M+ ARR) | **$249/mo Starter Plan** + 0.9% of billing volume (includes first $40k/mo billing volume at no charge) | **90-day free trial** on the Starter plan with full feature sandbox testing and zero platform charges during the trial window | Churn reduction, subscriber retention, predictive card renewal algorithms, and high-velocity consumer and B2B subscription billing. |
| **[Maxio](https://www.maxio.com/)** | PE-backed merger of Chargify & SaaSOptics (~$50M ARR) | **$599/mo** (Grow plan for up to $100k/mo in billing volume) | **Free developer sandbox ("Build")** with no live charging to test API integrations, billing logic, and financial configurations | Comprehensive financial operations for B2B SaaS combining subscription billing engine mechanics with GAAP/IFRS revenue recognition. |
| **[FastSpring](https://fastspring.com/)** | PE-backed (Accel-KKR / LLR Partners, $1B+ GMV processed) | Commission model: quote-based per-transaction fee (typically **3.9%–5.9% + $0.95/txn** or flat 8.9%) | **Free sandbox account** with $0 monthly platform subscription fee; fees apply only upon processed commercial transactions | Merchant of Record (MoR) and checkout solution specializing in global software, desktop apps, video games, and SaaS tax remittance. |
| **[Rebilly](https://www.rebilly.com/)** | Privately held (~$6M+ ARR) | **$125/mo** (Pro tier base fee) + 1% volume fee | **30-day free trial** plus permanent developer sandbox environment to test multi-gateway orchestration and payment logic | Subscription management featuring advanced payment orchestration, multi-gateway failover routing, and automated dunning/fraud prevention. |
| **[Ordway](https://ordwaylabs.com/)** | Series A venture-backed (~$12.5M funding, ~$5M ARR) | Mid-market custom contracts (starting at approximately **$1,000/mo to $1,500/mo**) | **No public self-serve free trial**; sandbox and demo instances available via sales consultation and guided onboarding | Billing and revenue automation handling hybrid pricing, usage metering, contract milestones, complex invoicing, and ERP integrations. |

---

## Open-Source GitHub Projects

Open-source recurring billing software provides self-hosted control, zero vendor lock-in, and custom pricing logic flexibility. Repositories below are ordered in descending order of GitHub stargazers:

### Full Billing Platforms & Metering Engines

- **[Hyperswitch](https://github.com/juspay/hyperswitch)** [![GitHub stars](https://img.shields.io/github/stars/juspay/hyperswitch?style=social&color=white)](https://github.com/juspay/hyperswitch/stargazers)  
  *High-performance, open-source payment orchestration platform written in Rust (Apache-2.0).* Connects to 100+ processors (Stripe, Adyen, Braintree) through a single unified API. Features intelligent transaction routing, smart retries, zero vendor lock-in, and native recurring payment vaults that pair seamlessly with subscription engines like Kill Bill.

- **[Lago](https://github.com/getlago/lago)** [![GitHub stars](https://img.shields.io/github/stars/getlago/lago?style=social&color=white)](https://github.com/getlago/lago/stargazers)  
  *Leading open-source usage-based and subscription billing engine (AGPL-3.0).* Engineered as a self-hosted alternative to Chargebee and Stripe Billing. Features high-scale usage event ingestion, billable metrics aggregation (`COUNT`, `SUM`, `MAX`, `WEIGHTED SUM`), hybrid pricing plans, automated invoicing, and customizable dunning flows.

- **[Flexprice](https://github.com/flexprice/flexprice)** [![GitHub stars](https://img.shields.io/github/stars/flexprice/flexprice?style=social&color=white)](https://github.com/flexprice/flexprice/stargazers)  
  *Open-source pricing and billing infrastructure built for modern AI applications and developer tools (Apache-2.0).* Enables engineering teams to run entitlement checks, track consumption-based metrics in real time, launch dynamic pricing tiers, and deploy entirely within their own cloud VPC.

- **[Kill Bill](https://github.com/killbill/killbill)** [![GitHub stars](https://img.shields.io/github/stars/killbill/killbill?style=social&color=white)](https://github.com/killbill/killbill/stargazers)  
  *The enterprise-standard open-source subscription billing and payments engine (Apache-2.0, in production since 2010).* Provides catalog and multi-phase plan configuration, subscription lifecycle handling (upgrades, pauses, proration), event-driven invoicing, payment gateway plugins, dunning, tax compliance connectors, and multi-tenant isolation. Includes the open-source **Kaui** admin dashboard.

- **[OpenMeter](https://github.com/openmeterio/openmeter)** [![GitHub stars](https://img.shields.io/github/stars/openmeterio/openmeter?style=social&color=white)](https://github.com/openmeterio/openmeter/stargazers)  
  *Cloud-native usage metering infrastructure for consumption billing (Apache-2.0).* Ingests millions of real-time application and AI token events with deduplication and sub-second window aggregation, exporting clean billing records directly into Stripe, Lago, or ERP engines.

- **[BillaBear](https://github.com/billabear/billabear)** [![GitHub stars](https://img.shields.io/github/stars/billabear/billabear?style=social&color=white)](https://github.com/billabear/billabear/stargazers)  
  *Open-source subscription management and billing system built on PHP/Symfony.* Provides self-hosted subscription lifecycles, automated tax calculations, customer self-service billing portals, dunning automation, and Stripe integration without proprietary lock-in.

- **[UniBee](https://github.com/UniBee-Billing/unibee)** [![GitHub stars](https://img.shields.io/github/stars/UniBee-Billing/unibee?style=social&color=white)](https://github.com/UniBee-Billing/unibee/stargazers)  
  *Lightweight open-source SaaS billing software (AGPL-3.0).* Positioned as an easy-to-deploy self-hosted billing system featuring product catalogs, recurring subscription flows, invoice creation, discount codes, merchant controls, and an end-user customer portal via Docker Compose.

- **[Billmora](https://github.com/Billmora/billmora)** [![GitHub stars](https://img.shields.io/github/stars/Billmora/billmora?style=social&color=white)](https://github.com/Billmora/billmora/stargazers)  
  *Open-source automated web hosting and server recurring billing platform built on Laravel (GPL-3.0).* Manages client renewals, periodic recurring invoices, service provisioning, and ticketed support operations.

### Payment Switching & Developer Primitives

- **[stapel-billing](https://github.com/stapel-io/stapel-billing)** — Django application providing immutable credit wallets, recurring subscriptions, Stripe checkout flows, and idempotent webhook handling for Python backends.
- **BillCycle** — Python/FastAPI billing engine utilizing event-sourcing and finite state machines for subscription models.

### Personal Subscription Trackers

- **[Wallos](https://github.com/ellite/Wallos)** [![GitHub stars](https://img.shields.io/github/stars/ellite/Wallos?style=social&color=white)](https://github.com/ellite/Wallos/stargazers) — Self-hostable web app for tracking personal subscriptions, recurring household expenses, and renewal alerts.
- **[Subscription-Manager](https://github.com/dh1011/subscription-manager)** [![GitHub stars](https://img.shields.io/github/stars/dh1011/subscription-manager?style=social&color=white)](https://github.com/dh1011/subscription-manager/stargazers) — Minimalist recurring expense and subscription tracker with calendar projections and push notifications.

---

## Choosing the Right Billing Stack

```
                                  What is your primary billing need?
                                                  │
                 ┌────────────────────────────────┴────────────────────────────────┐
                 ▼                                                                 ▼
     [ Developer-Led / Self-Hosted ]                                 [ Fully Managed / Turnkey SaaS ]
                 │                                                                 │
      ┌──────────┴──────────┐                                           ┌──────────┴──────────┐
      ▼                     ▼                                           ▼                     ▼
[ Open Source Engine ] [ Custom Gateway Routing ]             [ Merchant of Record ]    [ Billing & Invoicing ]
  • Lago (Usage/Hybrid)  • Hyperswitch (Multi-processor)        • Paddle (Global tax)     • Stripe Billing (API)
  • Kill Bill (Modular)  • stapel-billing (Django)              • FastSpring (Digital)    • Chargebee (RevRec)
  • Flexprice (AI/Usage)                                                                  • Zuora (Enterprise)
```

1. **Merchant of Record (MoR) vs. Billing Gateway:**
   - Choose an **MoR** (Paddle, FastSpring) if you want to offload worldwide sales tax, VAT/GST registration, and chargeback disputes entirely.
   - Choose a **Billing Platform** (Stripe Billing, Chargebee, Recurly) if you have registered legal business entities and prefer direct merchant processor relationships with lower per-transaction fees.
2. **Usage-Based & Metered Pricing:**
   - For consumption-driven AI, API, or compute workloads, choose specialized metering layers like **OpenMeter** or native usage engines like **Lago** and **Flexprice**.
3. **Open-Source Self-Hosting Considerations:**
   - Deploying open-source engines like **Kill Bill** or **Lago** gives you absolute data residency and removes revenue take-rates. However, you maintain responsibility for PCI-DSS compliance scope, database resilience, and payment gateway plugin security.

---

## How to Contribute

Contributions are welcome! Please follow these guidelines:

1. **Fork** this repository.
2. Create a new branch: `git checkout -b feature/add-billing-tool`.
3. Add your tool to the appropriate table or list with valid Markdown links, pricing specifics, or GitHub stars badge.
4. Ensure entries remain objective, factual, and free of sales marketing language.
5. Open a **Pull Request** explaining the additions.

---

## Disclaimer

This repository is maintained for educational and informational purposes. Product pricing, free tier limits, company valuations, and repository star metrics are subject to ongoing change by their respective providers. Always review official terms of service, PCI-DSS compliance requirements, and vendor documentation before implementing billing architecture in production.
