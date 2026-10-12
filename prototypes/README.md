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

**Question:** does a working IO CRM show the people who will use it the value the BRD promises?

This is a clickable demo of one working day for a Europe section lead, with a guided tour of 11 steps. Each step pairs a problem from the BRD's current-state analysis (Excel per section, WhatsApp, Outlook lists, manual HQ packs) with the CRM feature that solves it, then asks the viewer to try that feature: merge duplicates, read the history across sections, move the pipeline, complete an automatic follow-up, log an event meeting offline, capture a lead on a phone (card scan, duplicate check, consent, offline queue, sharing with stakeholders), track Abu Dhabi destination stakeholders across trade promotion activities (FR-C1), build a campaign segment, and switch to the leadership view of the HQ report. The final step checks the results against BRD §2.3 success criteria.

**Run:** open the file in a browser, or use the published Artifact link.
