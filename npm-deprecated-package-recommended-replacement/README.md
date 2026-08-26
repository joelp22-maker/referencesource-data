# Deprecated npm packages and their maintainer-named replacement

npm allows a maintainer to attach a 'deprecated' message to a specific published version, and that message often names the exact replacement package or built-in API to use instead -- 'left-pad' points at String.prototype.padStart(), 'istanbul' points at nyc, 'tslint' points at ESLint, 'babel-eslint' points at @babel/eslint-parser. This is first-party, machine-readable data sitting in the registry API itself, but nobody has assembled it into a browsable table: a developer running `npm install` sees the warning once in a terminal scroll and it is gone, and the alternative is a content-mill blog post ranking '10 request alternatives' without quoting what the maintainer actually said. This asset would have been too tedious to maintain by hand across thousands of packages -- watching a firehose of new deprecations and re-checking old ones for changes -- but is a mechanical registry read for one machine, refreshable on a schedule at zero marginal cost per package. Each record is one deprecated package, quoting its maintainer's own deprecated message verbatim and naming the specific replacement stated in it. Answers 'is request deprecated', 'what should I use instead of tslint', 'why is my npm install warning about gulp-util'.

**96 records.** Canonical, always-current version: [https://referencesource.org/npm-deprecated-package-recommended-replacement/](https://referencesource.org/npm-deprecated-package-recommended-replacement/)

| | |
|---|---|
| Last verified | 2026-08-25 |
| Re-check due | 2027-02-21 |
| Records | 96 |
| Machine-readable | [`data.json`](data.json) · [changes feed](https://referencesource.org/npm-deprecated-package-recommended-replacement/changes.xml) |

Every record carries `source` (the page it came from) and `source_quote` (the exact line on that page which states it), so any value here can be checked without asking us. Where a source does not state something the row is omitted rather than guessed.

**Licence position for this dataset.** Facts from the public npm registry API; package metadata is not a copyrightable compilation of the underlying facts

---

Snapshot of [referencesource.org](https://referencesource.org/npm-deprecated-package-recommended-replacement/), which is canonical and re-verified on a schedule. If a record here is wrong, that is worth more to us than one that is right — please open an issue.
