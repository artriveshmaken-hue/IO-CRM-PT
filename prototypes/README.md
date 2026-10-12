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

The scope is the BRD only. The IO operating summary was used for context.

Navigation is grouped by the work people do:

- **Overview:** Home (my day) and Market 360, a consolidated picture of All IO, a section or a country: performance against target joined with partners, pipeline, events, campaigns and engagement
- **Relationships:** Partners (FR-A1), Stakeholders (FR-C1), Pipeline (FR-A2) and Activities (FR-A3, FR-C3)
- **Promotion:** Trade promotion (FR-C1 to C4) and Campaigns (FR-B1 to B3)
- **Insights:** Reports (FR-A4, FR-C4, FR-D2) and BRD coverage

Partners, stakeholders and events open as full detail pages with tabs. For example, an event has Overview, Invitations, Stakeholders, Meetings & leads and Results.

The basics are covered: sign-in with four role-scoped personas (FR-D1, NFR 10), search, notifications, activity logging, record history, an EN / عربي switch, and mobile capture forms that work offline.

The guided tour has 9 steps and sits in a pinned bar under the top bar, so Back and Next are always visible. The app is locked to the viewport and only the content area scrolls. All data is fictional.

**Run:** open the file in a browser, or use the published Artifact link.
