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

**Question:** does a working IO CRM show the value of the BRD (DCT-IO-CRM-BRD v1.0) to the people who will use it?

The scope is the BRD only. The IO operating summary was used for context (sections, units, partner and event types).

- **Basics:** sign-in (DCT single sign-on, simulated) with four role-scoped personas (Section Lead Europe, Unit Head DACH, PR & Marketing Officer, IO Leadership & PMO); search; notifications; activity logging and record history; EN / عربي switch
- **Workstream A:** partner master with de-duplication (FR-A1); mobile lead capture and the Prospect → Active pipeline with a conversion trend (FR-A2); cadence rules creating and escalating follow-ups (FR-A3); partner and pipeline dashboards plus a personal view (FR-A4)
- **Workstream B:** segments synced to the existing newsletter tool (FR-B1); co-marketing per partnership (FR-B2); performance (FR-B3)
- **Workstream C:** destination stakeholders and events (FR-C1); invitations and mobile meeting logging that works offline (FR-C2); automatic post-event follow-up (FR-C3); cross-IO timeline and event return (FR-C4)
- **Workstream D:** row-level access (FR-D1); leadership view and an auto-generated monthly HQ pack (FR-D2)
- **BRD coverage page:** each requirement mapped to where it appears, plus the out-of-scope items and the open-item assumptions

A 12-step guided tour ends on the BRD §2.3 success criteria. All data is fictional.

**Run:** open the file in a browser, or use the published Artifact link.
