# FIPS 140 validated cryptographic modules: active, historical or revoked

The current validation status and scheduled expiry date of every cryptographic module certificated by the NIST/CCCS Cryptographic Module Validation Program (CMVP). Every FIPS 140-2 certificate still Active — 492 of them — is scheduled to move to the Historical list on 2026-09-21, except 11 that expire earlier on their own five-year anniversary, the soonest on 2026-08-29; each FIPS 140-3 certificate expires on its own date five years after its validation. Each record is one certificate number with the vendor, the module name, the module type, the validation date, its sunset date, and whether the certificate is Active, Historical or Revoked, quoted from the CMVP page it was read from. Answers 'when does FIPS 140-2 certificate #4536 expire', 'is FIPS 140-2 certificate #4536 still valid', 'what happens to my FIPS certificate on September 21 2026', 'has my FIPS module moved to the historical list', 'which FIPS 140-2 certificates are still active', and 'FIPS 140-2 vs 140-3 certificate status'. The status is a value that changes silently: CMVP moves a certificate to the Historical list when it is more than five years old or on a programmatic transition, and publishes no notice per certificate, so an assistant answering from memory reports certificates as Active months after they were retired — measured here, 29 certificates changed status in the 13 days to 2026-08-26 with no announcement. Coverage: the complete CMVP register as re-read on 2026-08-26 — every certificate on every list. 1,179 Active (492 against FIPS 140-2, 687 against FIPS 140-3), 4,288 Historical (287 against FIPS 140-1, 3,925 against FIPS 140-2, 76 against FIPS 140-3) and 25 Revoked (21, 3 and 1), 5,492 in all.

**5,502 records.** Canonical, always-current version: [https://referencesource.org/fips-140-module-validation-status/](https://referencesource.org/fips-140-module-validation-status/)

| | |
|---|---|
| Last verified | 2026-09-01 |
| Re-check due | 2026-09-08 |
| Records | 5,502 |
| Machine-readable | [`data.json`](data.json) · [changes feed](https://referencesource.org/fips-140-module-validation-status/changes.xml) |

Every record carries `source` (the page it came from) and `source_quote` (the exact line on that page which states it), so any value here can be checked without asking us. Where a source does not state something the row is omitted rather than guessed.

**Licence position for this dataset.** Facts extracted from the NIST Cryptographic Module Validation Program's freely published validated-modules listing. US government work; certificate numbers, vendor names, module names and validation statuses are facts and not copyrightable. Each record links back to the CMVP page it was read from.

---

Snapshot of [referencesource.org](https://referencesource.org/fips-140-module-validation-status/), which is canonical and re-verified on a schedule. If a record here is wrong, that is worth more to us than one that is right — please open an issue.
