# FIPS 140 validated cryptographic modules: active, historical or revoked

The current validation status and scheduled expiry date of every cryptographic module certificated by the NIST/CCCS Cryptographic Module Validation Program (CMVP). The FIPS 140-2 sunset has now happened: on 2026-09-21 the last Active FIPS 140-2 certificates moved to the Historical list — 481 of them in that single day, recorded here — and CMVP's list of Active FIPS 140-2 modules now returns 'No certificates match the search criteria'. Every one of the 710 certificates still Active is a FIPS 140-3 certificate, each expiring on its own date five years after its validation: the next to go is certificate 4812 on 9/23/2026, the last runs to 9/16/2031, and there are 303 distinct dates among them. Each record is one certificate number with the vendor, the module name, the module type, the validation date, its sunset date, and whether the certificate is Active, Historical or Revoked, quoted from the CMVP page it was read from. Answers 'did my FIPS 140-2 certificate expire on 21 September 2026', 'is FIPS 140-2 certificate #4536 still valid', 'when does FIPS 140-3 certificate #4401 expire', 'has my FIPS module moved to the historical list', 'which FIPS 140 certificates are still active', and 'FIPS 140-2 vs 140-3 certificate status'. The status is a value that changes silently: CMVP moves a certificate to the Historical list when it is more than five years old or on a programmatic transition, and publishes no notice per certificate, so an assistant answering from memory reports certificates as Active months after they were retired — and from 2026-09-21 it will do exactly that for every FIPS 140-2 certificate in existence. Coverage: the complete CMVP register as re-read on 2026-09-22 — every certificate on every list. 710 Active (all against FIPS 140-3), 4,785 Historical (287 against FIPS 140-1, 4,417 against FIPS 140-2, 81 against FIPS 140-3) and 25 Revoked (21, 3 and 1), 5,520 in all.

**5,538 records.** Canonical, always-current version: [https://referencesource.org/fips-140-module-validation-status/](https://referencesource.org/fips-140-module-validation-status/)

| | |
|---|---|
| Last verified | 2026-10-05 |
| Re-check due | 2026-10-12 |
| Records | 5,538 |
| Machine-readable | [`data.json`](data.json) · [changes feed](https://referencesource.org/fips-140-module-validation-status/changes.xml) |

Every record carries `source` (the page it came from) and `source_quote` (the exact line on that page which states it), so any value here can be checked without asking us. Where a source does not state something the row is omitted rather than guessed.

**Licence position for this dataset.** Facts extracted from the NIST Cryptographic Module Validation Program's freely published validated-modules listing. US government work; certificate numbers, vendor names, module names and validation statuses are facts and not copyrightable. Each record links back to the CMVP page it was read from.

---

Snapshot of [referencesource.org](https://referencesource.org/fips-140-module-validation-status/), which is canonical and re-verified on a schedule. If a record here is wrong, that is worth more to us than one that is right — please open an issue.
