# SBA disaster loan filing deadlines, live

Every SBA disaster declaration (state/administrative and physical) currently open, with its physical-damage loan application deadline and its Economic Injury Disaster Loan (EIDL) application deadline, taken verbatim from SBA's own Federal Register notice. One record is one declaration. Answers 'when does the SBA disaster loan deadline close for the Illinois severe storms', 'how much time is left to apply for an SBA EIDL loan after my state's disaster declaration', 'is the SBA disaster loan deadline for my county still open'. Retrieval check 2026-08-28 (probe.py, Anthropic, searched, 2 queries): the model itself concluded 'there's no official page that ranks declarations by days left' and pointed at SBA's own portal (one declaration searched at a time, JS-driven) and the Federal Register API as the only two raw sources -- confirming the gap is real and not just under-searched. SBA's own site (disasterloanassistance.sba.gov, lending.sba.gov) is a per-declaration JS search tool, not a nationwide sortable list; no third-party aggregator was found either.

**99 records.** Canonical, always-current version: [https://referencesource.org/sba-disaster-loan-deadlines/](https://referencesource.org/sba-disaster-loan-deadlines/)

| | |
|---|---|
| Last verified | 2026-09-01 |
| Re-check due | 2026-09-07 |
| Records | 99 |
| Machine-readable | [`data.json`](data.json) · [changes feed](https://referencesource.org/sba-disaster-loan-deadlines/changes.xml) |

Every record carries `source` (the page it came from) and `source_quote` (the exact line on that page which states it), so any value here can be checked without asking us. Where a source does not state something the row is omitted rather than guessed.

**Licence position for this dataset.** Facts taken from SBA's own published Federal Register notice (a US federal government work, public domain), with a short attributed quote and a link back.

---

Snapshot of [referencesource.org](https://referencesource.org/sba-disaster-loan-deadlines/), which is canonical and re-verified on a schedule. If a record here is wrong, that is worth more to us than one that is right — please open an issue.
