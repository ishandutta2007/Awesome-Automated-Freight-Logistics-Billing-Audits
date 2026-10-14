# Awesome-Automated-Freight-Logistics-Billing-Audits

## Top Automated Freight & Logistics Billing Audits Ecosystem



**Curated List of SaaS Products & Open-Source GitHub Projects**

*Focused on Freight Invoice Validation, Rate Compliance & Payment Automation*

**Last updated: March 2026**



This repository tracks notable **SaaS platforms** and **open-source projects** for **Automated Freight & Logistics Billing Audits**. These tools compare line-item carrier invoices against contracted rates, shipment records, and accessorial agreements—identifying overcharges, duplicate billings, and billing errors before payment is released.



**Examples** include Loop, Trax Technologies, Cass Information Systems, enVista, DDC FPO, Transmetrics, Intramotev, FreightVerify, ShipERP, and Zero Down Supply Chain (the category leaders).



**Open-source emphasis**: This section is heavily expanded with every major active project for self-hosting, deterministic reconciliation engines, and open TMS infrastructure—ideal for shippers, freight brokers, and developers seeking transparent, vendor-independent freight audit.



Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.



## Table of Contents

- [SaaS/Hosted Platforms](#saas-hosted-platforms)

- [Open-Source GitHub Projects](#open-source-github-projects)

- [How to Contribute](#how-to-contribute)

- [Disclaimer](#disclaimer)



## SaaS/Hosted Platforms



- **[Loop](https://www.loop.com/)**

  AI-native Logistics Data Platform recognized in the 2026 Gartner® Market Guide for Freight Audit and Payment Providers. Built on a full-stack AI data foundation with proprietary model **Dux™** for automated transportation data extraction. Merger with Data2Logistics and acquisition of StrategIQ Commerce expanded freight under management across parcel management, real-time visibility, and global payment execution. **Control Suite** (Policies + Control Tower) turns billing standards into transparent, enforceable rules—automatically approving clean invoices and flagging only exceptions that matter .



- **[Trax Technologies](https://www.traxtech.com/)**

  Global freight audit and payment platform processing $24+ billion in annual transportation spend across 21,000+ carriers. AI models trained on 25+ years of normalized freight data. Multi-modal support (ocean, air, ground, rail). ERP integration with SKU-level cost allocation and automated cost center mapping. Trax AI and LLM technology reads and ingests data from various freight document types for pattern identification and strategic recommendations. Named to Inbound Logistics 2026 Top 100 Logistics & Supply Chain Technology Providers .



- **[Cass Information Systems](https://www.cassinfo.com/)**

  Six decades in freight audit and payment with $37 billion in annual processed freight spend. Processes and pays 35 million freight invoices each year across 15,000+ carriers in 114 currencies. Wholly owned subsidiary **Cass Commercial Bank** provides regulated payment security (SOC 1 Type II, U.S. Federal Reserve regulated). Services include rate management, EDI setup, exception handling, accruals and GL coding, carrier support, and invoice automation. CassPort® client portal for global visibility .



- **[enVista](https://www.envistacorp.com/)**

  ATOM (Advanced Transportation Optimization and Management) platform blending freight audit, payment solutions, TMS implementation, and business analytics. Processes $7B+ in freight invoices across thousands of carriers. Proprietary all-modes rating engine ensures optimal rates. Audit capabilities cover guaranteed service compliance, refund recovery, discount verification, incorrect class rating, accessorial charges, freight terms, duplicate charges, and mathematical extension errors. Executive dashboard for KPIs .



- **[DDC FPO](https://www.ddcfpo.com/)**

  Freight-focused BPO processing approximately 300,000 shipments per day across 33 countries—responsible for **one-third of North America's freight bills**. Serves 50% of motor carriers ranked by revenue. **iCapture** uses intelligent data capture to extract data from any document (invoices, freight bills, contracts, letters), classify by context, and verify without human intervention. Freight Rate Auditing validates carrier billing against contracted rates .



- **[Transmetrics](https://transmetrics.ai/)**

  AI data-and-intelligence layer for logistics sitting on top of existing TMS, telematics, and ERP systems. **SpotLoad** for spot-load profitability, **FleetMetrics** for fleet analytics, **AssetMetrics** for container forecasting, and **NetMetrics** for AI-powered linehaul planning. ISO/IEC 27001 and ISO 9001 certified, GDPR-compliant, EU-hosted. Speedy (DPD Bulgaria) achieved 82% linehaul utilization (up from 72%) with 7-9% total transportation cost reduction .



- **[FreightVerify](https://www.freightverify.com/)**

  Real-time visibility platform specialized in complex supply chain management. Enterprise-level integration for real-time tracking with ETA prediction and performance assessment. VinView product provides live tracking of incoming inventory—users report 90% confidence in delivery ETAs (up from 40%). Covers part order through consolidation, warehousing, cross-docking, and destination .



- **[ShipERP](https://www.shiperp.com/)**

  SAP-certified shipping solution with freight auditing of shipper carrier invoices, rate quoting, multi-carrier shipping, automatic track & trace, and denied party screening. Integrates directly into SAP ERP delivery transactions (VL02N). AES direct integration for electronic export information filing. Requires SAP ECC 6.0 EhP 0 or S/4HANA 1610 .



- **[Zero Down Supply Chain](https://www.zdscs.com/)**

  Specializes in identifying and reducing transportation and supply chain costs through Audit, Business Intelligence, Optimization, and TMS offerings. Proprietary **FreightOptics** software reduces erroneous shipping charges. Services all modes—Courier, Small Parcel, LTL, Truckload, International Air, Ocean, and direct Ocean Contracts. Reviewers praise "quick, transparent setup experience with strong focus on partnership" and "clear, accurate and reliable billing information" .



- **[Intramotev](https://www.intramotev.com/)**

  Autonomous railcar technology with **TugVolt** independently driven freight wagons. Signed commercial agreement with ÖBB Rail Cargo Group (RCG) to operate TugVolt railcars in Austria under the SARI initiative for first- and last-mile operations. RCG runs 1,000+ freight trains daily across 18 countries. Deployments in U.S. include Watco (Illinois) and R.J. Corman (Memphis Line, Kentucky) .



## Open-Source GitHub Projects



- **[Hermes Freight Reconciliation Plugin](https://hermes-agent.nousresearch.com/docs/zh-Hans/plugins/freight-reconciliation)**

  Payer-side freight reconciliation plugin for Hermes Agent (MIT). Imports carrier bills and trip ledgers into a **deterministic local core** (SQLite, WAL, no cloud), re-calculates against contracted rates, and produces **evidence-linked difference lists** for human review. **14 MCP tools** over uvx stdio. **Never approves payments, sends messages, or writes back to ERP/TMS**—final confirmations route through a local admin page the model cannot reach. Amounts are integer minor units; unknown is null, never 0. Jobs left QUEUED/RUNNING are marked FAILED/RUN_INTERRUPTED on startup with recovery_action. Inputs frozen by digest for deterministic re-runs .



- **[Trenova](https://github.com/emoss08/Trenova)**

  Source-available transportation management system for small and mid-sized over-the-road carriers (Fair Source Functional Source License). Written in Go, PostgreSQL, GraphQL, and React. Covers full order-to-cash cycle: shipment entry, dispatch, driver assignment, **rating and accessorials** (formula-based rate calculation, fuel surcharge, detention rules), **billing and invoicing** (billing readiness checks, invoice generation, adjustments), accounting, and compliance. EDI 204/210/214/990/997 partner workflows, telematics (Samsara), PC*MILER, AS2. Self-hostable on single Linux host with Docker Compose. **Pre-release software—not yet suitable for production use** .



### Additional Strong Open-Source Options



- **[OpenBoxes](https://github.com/openboxes/openboxes)** — Open-source supply chain and inventory management (EPL-1.0) with purchase order and shipment tracking adaptable for freight reconciliation.

- **[Odoo](https://github.com/odoo/odoo)** — Open-source business suite (LGPL-3.0) with Purchase, Inventory, and Accounting modules for freight cost allocation.

- **[ERPNext](https://github.com/frappe/erpnext)** — Open-source ERP (GPL-3.0) with Purchase Order and Accounts Payable modules for freight invoice processing.

- Community **n8n** workflows for freight invoice routing, carrier rate comparison, and audit alerting.



**Frameworks for building custom systems**: Combine **Hermes Freight Reconciliation Plugin** for deterministic payer-side audit with **Trenova** for carrier-side rating and billing, **OpenBoxes** for shipment tracking, and **PostgreSQL** for persistence—creating a fully self-hosted, enterprise-grade freight audit platform.



## How to Contribute



1. Fork the repo.

2. Add/edit entries in `README.md` (follow existing format).

3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.

4. Submit PR with a short explanation.



Star the repo if you find it useful!



## Disclaimer



- This is a **community-curated** list — not exhaustive and not an endorsement.

- Freight audit systems handling carrier invoices and payment data must comply with financial regulations and data protection requirements (GDPR, CCPA, etc.).

- **Payment execution requires regulated infrastructure.** Third-party audit providers like Cass operate through wholly owned commercial banks for payment security. Self-hosted open-source solutions should never approve payments or write back to ERP/TMS systems without human confirmation—the Hermes freight-reconciliation plugin explicitly routes final approvals through a local admin page the model cannot reach .

- **Deterministic reconciliation is the correct pattern.** The Hermes plugin pins its engine to an immutable commit and freezes inputs by digest so re-runs are reproducible. Amounts are integer minor units with null (not 0) for unknown values—this prevents silent data corruption .

- Self-hosted open-source solutions require proper security hardening, EDI connectivity, and ongoing maintenance. Trenova is explicitly pre-release and not production-ready .



---



**Made for shippers, freight brokers, logistics engineers, and developers building transparent freight audit solutions.**

Let's make Automated Freight & Logistics Billing Audits more open, data-driven, and deterministic.
