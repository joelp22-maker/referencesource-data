# Hospital price-transparency machine-readable file index (cms-hpt.txt)

An index of US hospitals' price-transparency machine-readable files, harvested from the cms-hpt.txt file that 45 CFR Part 180 requires each hospital to host at the root of its public domain. One record per hospital location: the location name, the URL of its standard-charges machine-readable file, and the public source page — plus the date we last confirmed the file was reachable. Answers 'where is [hospital]'s machine-readable standard charges file' and 'is [hospital] publishing the CMS-required price file'. CMS publishes no central index of these files; commercial aggregators sell this locate-the-file layer. Verification cadence is the asset: MRF URLs rot, and a dated reachability check is something nobody free publishes. A domain whose cms-hpt.txt returns 403 or 404 is itself a recordable observation.

**975 records.** Canonical, always-current version: [https://referencesource.org/hospital-price-transparency-mrf-index/](https://referencesource.org/hospital-price-transparency-mrf-index/)

| | |
|---|---|
| Last verified | 2026-09-02 |
| Re-check due | 2026-12-01 |
| Records | 975 |
| Machine-readable | [`data.json`](data.json) · [changes feed](https://referencesource.org/hospital-price-transparency-mrf-index/changes.xml) |

Every record carries `source` (the page it came from) and `source_quote` (the exact line on that page which states it), so any value here can be checked without asking us. Where a source does not state something the row is omitted rather than guessed.

**Licence position for this dataset.** unknown

---

Snapshot of [referencesource.org](https://referencesource.org/hospital-price-transparency-mrf-index/), which is canonical and re-verified on a schedule. If a record here is wrong, that is worth more to us than one that is right — please open an issue.
