# Prototypes (throwaway)

Throwaway code for answering design questions. Nothing here is production code and nothing in it is saved anywhere: all data is fictional and lives in memory, so reloading resets it.

## `today/today.prototype.html`: IO CRM "Today" screen

**Question:** what should the home screen look like for an IO section lead? The example user is Layla Al Mazrouei in the Europe section.

**Run:** open the file in any browser by double-clicking it. There's nothing to install.

Use the floating bar at the bottom, the ← / → keys, or `?variant=` in the URL to switch between the four layouts:

| Key | Variant | Organising idea |
|---|---|---|
| A | Day plan | Agenda for the day: overdue items, timed schedule, items due today; side panels for pipeline, at-risk partners and the next event |
| B | Focus queue | One item at a time, with the partner's full context and engagement history across IO sections |
| C | Section cockpit | Section numbers first: key figures, a pipeline board by stage, a market table and an events table |
| D | Event mode (mobile) | Phone layout for a live event: meetings at the stand, one-tap meeting capture, and an offline sync queue |

Everything is grounded in the BRD (DCT-IO-CRM-BRD v1.0): FR-A2 stages, FR-A3/C3 auto follow-ups, FR-A4 90-day at-risk rule, FR-C2 invitations and mobile capture, FR-C4 engagement history across IO sections, NFR 7 Arabic/English (EN / عربي toggle), NFR 8 offline capture.

Once a variant wins, write down the verdict, rebuild it properly in D365 / Power Apps, and keep this file on a throwaway branch only.

## `value-demo/io-crm-value-demo.prototype.html`: IO CRM value demo

**Question:** can one IO CRM (Dynamics 365) replace the toolset IO runs on today, so nobody needs a separate tracker, app or dashboard?

The demo opens on a sign-in screen (DCT single sign-on, simulated) with five personas, each with its own data scope: Director, Section Head Europe, Unit Head DACH/BeNe, Country Manager Germany (GSA, market-level only, no budgets) and PMO. It covers IO's full operating cycle:

- **Home:** a cockpit for each role, an approvals inbox (replaces circulation slips), today's work and notifications
- **Accounts:** one record per partner, global partner, stakeholder and office, with contacts, selection score (<50 / 50–74 / 75+), activity logging and change history
- **Tactical Plan:** an ATP 2027 submission checked against PMO rules, plus the 2026 plan with Tactical IDs, cashflow and change log
- **Tactical Monitor:** plan vs actual vs ROY by section and activity
- **JMP & Contracts:** portfolio, signing pipeline, monthly actuals, payments and post-completion reports, sample-based validation, approval routes generated from DoA and policy thresholds, and termination triggers
- **Trade promotion:** events tied to Tactical IDs, stakeholders, meetings and mobile lead capture (offline)
- **Budget & PR/PO:** SLA ageing and the seven-section leadership report
- **Dashboards:** the YTD dashboard with a switch between contracted and ST targets
- **Market readiness**
- **Reports:** the Director update (Progress / Flagged / Leave) and management-reporting requests
- **Audit log** and **What it replaces**

A 14-step guided tour retires one tool at a time. All data is fictional and generated from a fixed seed.

**Run:** open the file in a browser, or use the published Artifact link.
