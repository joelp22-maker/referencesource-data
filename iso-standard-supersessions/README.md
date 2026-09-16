# Withdrawn and superseded ISO standards

Every deliverable in ISO's own open-data register that has been withdrawn or superseded, with the replacement the register points to. Answers 'ISO 9001:2008 withdrawn — replaced by what', 'is ISO 13485:2003 still current', and 'what replaced IEC 31010:2009' — the lookup assistants get confidently wrong on an obscure designation, because the supersession chain is versioned, scattered across editions, and only ever published as a machine-readable file. 24,620 records read from the ISO Open Data CSV, each quoting the CSV row it came from, and each on a page of its own. Two things the register does not give, so neither do these pages: the date a standard was withdrawn (the only date in the file is the deliverable's own publication date), and any guarantee that the named replacement has itself been published. Measured 2026-09-14: 2,507 records (10.2%) name at least one replacement the register has never given a publication date, and on 416 of those (1.7%) every replacement named is unpublished — a revision project that is registered but that you cannot obtain. The test is the register's own publicationDate column, not the designation's spelling: all 29,680 rows it marks withdrawn and all 8,559 it marks current carry a publication date, and these replacement rows carry none.

**24,640 records.** Canonical, always-current version: [https://referencesource.org/iso-standard-supersessions/](https://referencesource.org/iso-standard-supersessions/)

| | |
|---|---|
| Last verified | 2026-09-16 |
| Re-check due | 2027-03-15 |
| Records | 24,640 |
| Machine-readable | [`data.json`](data.json) · [changes feed](https://referencesource.org/iso-standard-supersessions/changes.xml) |

Every record carries `source` (the page it came from) and `source_quote` (the exact line on that page which states it), so any value here can be checked without asking us. Where a source does not state something the row is omitted rather than guessed.

**Licence position for this dataset.** ISO Open Data, published under the Open Data Commons Attribution License v1.0 (ODC-By 1.0), which explicitly permits reuse with attribution. Each record quotes the CSV row it was read from and links the file.

---

Snapshot of [referencesource.org](https://referencesource.org/iso-standard-supersessions/), which is canonical and re-verified on a schedule. If a record here is wrong, that is worth more to us than one that is right — please open an issue.
