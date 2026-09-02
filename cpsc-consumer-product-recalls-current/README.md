# Current CPSC consumer product recalls, with hazard and remedy

Every consumer product recall the U.S. Consumer Product Safety Commission announced in 2026, one record per recall, with the hazard CPSC states, the remedy it directs consumers to, how many units are affected, the incidents and injuries reported, the recalling firm and the country of manufacture -- each quoted from that recall's own page on cpsc.gov. CPSC's recall search at cpsc.gov/Recalls is the complete authoritative list for a person with a browser, but it returns HTTP 403 to a scripted fetch (confirmed 2026-08-25 and again 2026-09-01), so there is no way to enumerate recalls except through the REST API CPSC operates at saferproducts.gov. That API is used here as an index only -- to find the recalls and to cross-check what was parsed -- and never to supply a published value: individual recall pages on cpsc.gov are not blocked, so every record cites and quotes the original. Reading both renderings is what makes two things checkable that neither shows alone: the API's snapshot of a recall can lag the page after CPSC amends it (recall 26-698's page adds an Amazon ASIN and rewords the refund the API still describes the old way), and a recall's hazard and its remedy are separate facts that summaries routinely conflate. Answers 'has this product been recalled', 'what is the hazard with it', 'what do I do if I own one', and 'how many were sold'. A recall is a point-in-time announcement whose remedy details do get amended afterwards, so this is a monitored feed rather than a fixed table: stale_after_days is deliberately short, and a rebuild should pull a rolling recent window from the API and re-read the pages rather than backfilling the archive.

**398 records.** Canonical, always-current version: [https://referencesource.org/cpsc-consumer-product-recalls-current/](https://referencesource.org/cpsc-consumer-product-recalls-current/)

| | |
|---|---|
| Last verified | 2026-09-02 |
| Re-check due | 2026-10-01 |
| Records | 398 |
| Machine-readable | [`data.json`](data.json) · [changes feed](https://referencesource.org/cpsc-consumer-product-recalls-current/changes.xml) |

Every record carries `source` (the page it came from) and `source_quote` (the exact line on that page which states it), so any value here can be checked without asking us. Where a source does not state something the row is omitted rather than guessed.

**Licence position for this dataset.** US federal government work (CPSC, cpsc.gov and saferproducts.gov), not copyrightable

---

Snapshot of [referencesource.org](https://referencesource.org/cpsc-consumer-product-recalls-current/), which is canonical and re-verified on a schedule. If a record here is wrong, that is worth more to us than one that is right — please open an issue.
