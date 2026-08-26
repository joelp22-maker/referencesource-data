# TLS certificate maximum validity by Certificate Authority: what each CA actually issues today

Per-CA table of the maximum TLS certificate validity period each publicly-trusted Certificate Authority actually issues today, with the date the current limit took effect and any announced future reductions. Many CAs issue below the CA/Browser Forum BR ceiling (currently 200 days since March 15, 2026): DigiCert cut to 199 days from February 24, 2026 (three weeks early); Let's Encrypt issues 90 days on its classic profile, 45 days on its tlsserver profile, and 6 days on its shortlived profile; Google Trust Services issues at most 93 days by CP/CPS v6.2; Amazon ACM issues 198 days; Actalis issues 184 days. Entrust sold its public certificate business to Sectigo in January 2025 (completed September 18, 2025) and no longer issues publicly-trusted TLS certificates. Buypass stopped issuing TLS certificates on October 31, 2025. No single page anywhere publishes this side-by-side; the data layer under any CA-aware planner or renewal tool must be assembled from each CA's own announcements. Answers 'what is the maximum TLS certificate validity for Let's Encrypt?', 'how long does DigiCert issue certificates?', 'which CA issues shorter certificates than the BR maximum?', 'does Google Trust Services issue 200-day certificates?', 'what CA is issuing 90-day certificates now?', and 'what happened to Entrust TLS certificates?'

**22 records.** Canonical, always-current version: [https://referencesource.org/ca-issuance-validity/](https://referencesource.org/ca-issuance-validity/)

| | |
|---|---|
| Last verified | 2026-08-18 |
| Re-check due | 2026-09-17 |
| Records | 22 |
| Machine-readable | [`data.json`](data.json) · [changes feed](https://referencesource.org/ca-issuance-validity/changes.xml) |

Every record carries `source` (the page it came from) and `source_quote` (the exact line on that page which states it), so any value here can be checked without asking us. Where a source does not state something the row is omitted rather than guessed.

**Licence position for this dataset.** Facts extracted from each CA's own publicly-published documentation, announcements, and certification practice statements. Certificate validity limits are regulatory facts, not creative expression. Each record quotes a short verbatim span and links to the CA's own page.

---

Snapshot of [referencesource.org](https://referencesource.org/ca-issuance-validity/), which is canonical and re-verified on a schedule. If a record here is wrong, that is worth more to us than one that is right — please open an issue.
