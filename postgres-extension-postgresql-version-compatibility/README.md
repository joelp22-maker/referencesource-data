# PostgreSQL extension compatibility with PostgreSQL major versions

Which major versions of PostgreSQL a popular server extension supports, taken from that extension's own documentation, README or changelog -- not from any one cloud vendor's managed-service certification list. Before upgrading a self-hosted PostgreSQL server, an operator running several extensions has to check every extension's supported range separately, because dropping support for an old PostgreSQL version and adding support for a new one happen on each extension's own schedule, not in step with Postgres itself or with each other. Cloud vendors (Azure, AWS/Aurora, DigitalOcean, Alibaba) each publish their own extension-by-version table, but that shows what the vendor has certified for its managed service, which lags or diverges from what the extension's own maintainers say it supports; no vendor-neutral page was found that cites each extension's own documentation. Some projects state a range in one sentence; others state only that a particular release added or dropped a PostgreSQL version, and the range has to be read off those entries. Both are recorded here, and which one a record rests on is visible from its quote.

**9 records.** Canonical, always-current version: [https://referencesource.org/postgres-extension-postgresql-version-compatibility/](https://referencesource.org/postgres-extension-postgresql-version-compatibility/)

| | |
|---|---|
| Last verified | 2026-09-02 |
| Re-check due | 2026-12-29 |
| Records | 9 |
| Machine-readable | [`data.json`](data.json) · [changes feed](https://referencesource.org/postgres-extension-postgresql-version-compatibility/changes.xml) |

Every record carries `source` (the page it came from) and `source_quote` (the exact line on that page which states it), so any value here can be checked without asking us. Where a source does not state something the row is omitted rather than guessed.

**Licence position for this dataset.** unknown

---

Snapshot of [referencesource.org](https://referencesource.org/postgres-extension-postgresql-version-compatibility/), which is canonical and re-verified on a schedule. If a record here is wrong, that is worth more to us than one that is right — please open an issue.
