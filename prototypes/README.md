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
