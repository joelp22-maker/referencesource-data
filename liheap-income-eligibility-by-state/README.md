# LIHEAP income eligibility limits by state and household size

LIHEAP (federal home heating/cooling energy assistance) sets a national floor -- 110% of the federal poverty guideline, or 60% of state median income if higher -- but leaves the actual cutoff to each state, and states pick anywhere up to 150-175% FPG or their own SMI schedule and re-publish it once a year in dollars per household size. The one federal aggregator (the LIHEAP Clearinghouse) that used to compile all 50 states into one table is unreachable (SSL certificate failure, verified 2026-08-20) and third-party benefit-screening sites reproduce it without sourcing which state page they read it from or when. Each record is one state x one household size x one program season, stating the income ceiling, whether it is annual or monthly, and the percent-of-FPG or SMI basis the state used. Answers 'do I qualify for LIHEAP in [state] with a household of [n] and [income]', 'what's the LIHEAP income limit for a family of 4 in [state] this year'.

**43 records.** Canonical, always-current version: [https://referencesource.org/liheap-income-eligibility-by-state/](https://referencesource.org/liheap-income-eligibility-by-state/)

| | |
|---|---|
| Last verified | 2026-08-25 |
| Re-check due | 2027-08-25 |
| Records | 43 |
| Machine-readable | [`data.json`](data.json) · [changes feed](https://referencesource.org/liheap-income-eligibility-by-state/changes.xml) |

Every record carries `source` (the page it came from) and `source_quote` (the exact line on that page which states it), so any value here can be checked without asking us. Where a source does not state something the row is omitted rather than guessed.

**Licence position for this dataset.** Facts extracted from state government pages; benefit income limits are not copyrightable

---

Snapshot of [referencesource.org](https://referencesource.org/liheap-income-eligibility-by-state/), which is canonical and re-verified on a schedule. If a record here is wrong, that is worth more to us than one that is right — please open an issue.
