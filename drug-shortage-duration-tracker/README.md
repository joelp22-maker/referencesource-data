# FDA drug shortage duration tracker

For every package FDA currently lists as in shortage: how long that shortage entry has been open (from openFDA's own `initial_posting_date` to today), what FDA says the package's supply is right now, and any recovery estimate FDA has given. What FDA itself publishes, checked directly on 2026-09-01 rather than assumed: the shortage list page (accessdata.fda.gov/scripts/drugshortages) shows which drugs are short and why and carries no date at all, while each per-drug detail page adds a single 'Date first posted' for the whole drug. Neither prints an elapsed duration, and neither gives the date per manufacturer. openFDA does — where several manufacturers report a shortage of the same drug, each carries its own posting date, and FDA's page shows only the earliest of them. Cross-checked across 30 drugs against those detail pages: 30 of 30 agreed, and in all 10 multi-manufacturer cases FDA's single date was exactly the earliest of ours. The underlying facts are FDA's own public-domain data; the duration is a computation over them that nobody publishes maintained, because it changes every day and hand-updating it was never worth the effort. A scheduled refetch of the same public API keeps it current for free. Read the duration next to `availability`, and do not read it alone: a shortage entry stays 'Current' until FDA resolves the whole shortage, so 63.8% of listed packages (746 of 1,169, measured 2026-09-01) are marked 'Available' even while their entry has been open for years — the median entry has been open 1,721 days and 1,118 of 1,169 have been open more than 1,000. Records cite a per-drug, per-manufacturer API query rather than a page offset, because openFDA's result ordering rotates daily and an offset URL stops containing its own record — see sources.txt. Source: https://api.fda.gov/drug/shortages.json (openFDA, no API key required at this volume). This is a monitored dataset, not a static page — stale_after_days is short and a build should re-run the fetch on a schedule rather than once.

**1,169 records.** Canonical, always-current version: [https://referencesource.org/drug-shortage-duration-tracker/](https://referencesource.org/drug-shortage-duration-tracker/)

| | |
|---|---|
| Last verified | 2026-09-01 |
| Re-check due | 2026-09-04 |
| Records | 1,169 |
| Machine-readable | [`data.json`](data.json) · [changes feed](https://referencesource.org/drug-shortage-duration-tracker/changes.xml) |

Every record carries `source` (the page it came from) and `source_quote` (the exact line on that page which states it), so any value here can be checked without asking us. Where a source does not state something the row is omitted rather than guessed.

**Licence position for this dataset.** openFDA drug shortage data is a U.S. government work and is in the public domain. No source-licence question arises; each record still cites the specific API query and retrieval date it came from.

---

Snapshot of [referencesource.org](https://referencesource.org/drug-shortage-duration-tracker/), which is canonical and re-verified on a schedule. If a record here is wrong, that is worth more to us than one that is right — please open an issue.
