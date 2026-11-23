# Can I put regulated data in this cloud service? What the vendor's own page says, and the government's own FedRAMP file

One record per named cloud service, answering the question a developer actually puts to a coding assistant: 'can I put patient data in X?' and 'is X FedRAMP authorised?'. Each record carries two separate things, from two separate publishers, and never mixes them: whether the vendor's own page names that service on its list of services covered by its HIPAA business associate agreement (BAA), quoted verbatim with the date the vendor last updated the list; and what the US General Services Administration's own daily FedRAMP export says about the status, impact level, authorisation date and authorisation type of the cloud service offering that service's vendor holds. Answers 'is Cloud Run covered by Google's HIPAA BAA', 'is BigQuery HIPAA eligible', 'does Microsoft sign a BAA for Azure', 'is OpenAI's web search HIPAA eligible' (the vendor's own answer is no), 'what FedRAMP impact level is Google Cloud authorised at', and 'which Google Workspace services are in the Google Cloud BAA'. The reason this is a dataset and not a memory is that the lists move: Google's own page stamped its Google Cloud list 2026-11-11, its SecOps list 2026-11-09 and its Workspace list 2026-10-28, three different dates on one page, and a service is added to or dropped from such a list without an announcement. NOTHING HERE SAYS A SYSTEM IS COMPLIANT, and nothing here says a reader may put protected health information anywhere. It says what the publisher's page says, with the sentence and the date, which is a different thing and the only thing that can be published honestly.

**173 records.** Canonical, always-current version: [https://referencesource.org/cloud-service-hipaa-baa-and-fedramp-status/](https://referencesource.org/cloud-service-hipaa-baa-and-fedramp-status/)

| | |
|---|---|
| Last verified | 2026-11-23 |
| Re-check due | 2026-12-23 |
| Records | 173 |
| Machine-readable | [`data.json`](data.json) · [changes feed](https://referencesource.org/cloud-service-hipaa-baa-and-fedramp-status/changes.xml) |

Every record carries `source` (the page it came from) and `source_quote` (the exact line on that page which states it), so any value here can be checked without asking us. Where a source does not state something the row is omitted rather than guessed.

**Licence position for this dataset.** Three publishers. The GSA's FedRAMP export is a US government work in the public domain and each record links to the exact file URL it was read from. Google's and Microsoft's pages are quoted as short attributed passages with a link back, which is the licence position in docs/constitution.md; both hosts' robots files and terms pages were read on 2026-11-23 through tools/ethics.py and neither forbids automated collection or use for AI systems. OpenAI's documentation page was read the same way on the same day with the same answer. AWS, Vercel and Supabase were refused by that gate and have no records here; see _not_included. No SOC 2, ISO/IEC 27001 or PCI DSS text appears anywhere in this dataset.

---

Snapshot of [referencesource.org](https://referencesource.org/cloud-service-hipaa-baa-and-fedramp-status/), which is canonical and re-verified on a schedule. If a record here is wrong, that is worth more to us than one that is right — please open an issue.
