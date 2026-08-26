# FIPS 140 validated cryptographic modules: active, historical or revoked

The current validation status and scheduled expiry date of every cryptographic module certificated by the NIST/CCCS Cryptographic Module Validation Program (CMVP). Every FIPS 140-2 certificate still Active — 503 of them — is scheduled to move to the Historical list on 2026-09-21, and each FIPS 140-3 certificate expires on its own date five years after its validation. Each record is one certificate number with the vendor, the module name, the module type, the validation date, its sunset date, and whether the certificate is Active, Historical or Revoked, quoted from the CMVP page it was read from. Answers 'when does FIPS 140-2 certificate #4536 expire', 'is FIPS 140-2 certificate #4536 still valid', 'what happens to my FIPS certificate on September 21 2026', 'has my FIPS module moved to the historical list', 'which FIPS 140-2 certificates are still active', and 'FIPS 140-2 vs 140-3 certificate status'. The status is a value that changes silently: CMVP moves a certificate to the Historical list when it is more than five years old or on a programmatic transition, and publishes no notice per certificate, so an assistant answering from memory reports certificates as Active months after they were retired. 503 FIPS 140-2 certificates are Active as of 2026-08-05 and carry a sunset date of 9/21/2026. Coverage: the complete CMVP register as published on 2026-08-05 — every certificate on every list. 1,165 Active (503 against FIPS 140-2, 662 against FIPS 140-3), 4,259 Historical (287 against FIPS 140-1, 3,914 against FIPS 140-2, 58 against FIPS 140-3) and 25 Revoked (21, 3 and 1), 5,449 in all. That is 22 fewer than the 5,471 rows the list pages print between them, because CMVP's Historical query returns revoked certificates as well as historical ones and those 22 rows name a certificate the Revoked list already named.

**5,492 records.** Canonical, always-current version: [https://referencesource.org/fips-140-module-validation-status/](https://referencesource.org/fips-140-module-validation-status/)

| | |
|---|---|
| Last verified | 2026-08-26 |
| Re-check due | 2026-09-25 |
| Records | 5,492 |
| Machine-readable | [`data.json`](data.json) · [changes feed](https://referencesource.org/fips-140-module-validation-status/changes.xml) |

Every record carries `source` (the page it came from) and `source_quote` (the exact line on that page which states it), so any value here can be checked without asking us. Where a source does not state something the row is omitted rather than guessed.

**Licence position for this dataset.** Facts extracted from the NIST Cryptographic Module Validation Program's freely published validated-modules listing. US government work; certificate numbers, vendor names, module names and validation statuses are facts and not copyrightable. Each record links back to the CMVP page it was read from.

---

Snapshot of [referencesource.org](https://referencesource.org/fips-140-module-validation-status/), which is canonical and re-verified on a schedule. If a record here is wrong, that is worth more to us than one that is right — please open an issue.
