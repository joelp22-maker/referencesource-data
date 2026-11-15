# Security and compliance controls, one provision at a time: NIST SP 800-53 and the HIPAA Security Rule in their own words

Every control in NIST SP 800-53 Rev 5 and every paragraph of the HIPAA Security Rule, cut one provision at a time, each with the publisher's own words as the record's quote. One record is one obligation: a control with five lettered statements becomes five records, keyed the way the publisher cites them (SC-28, SC-28(1), AC-2a, 164.312(a)(2)(iv)), so a reader or an agent that has been handed a control number gets that control's text and nothing else. Answers 'what does NIST SP 800-53 SC-28 require', 'what does HIPAA 164.312(a)(2)(iv) actually say about encryption', 'which published controls cover audit logging', and 'what is the organization-defined parameter in AC-12'. The hard part is not finding the documents — NIST publishes the catalogue as machine-readable OSCAL and the eCFR publishes the rule as XML — it is that both are published as whole documents, so a coding assistant asked to implement 'SC-28' either reads a 1,200-page catalogue or guesses. This dataset is the retrieval layer: provision in, the publisher's sentence out. It does not say how to implement anything; the control's own text is the whole of what is published here. NIST's machine-readable text leaves a placeholder where a value is the organisation's to decide ('Protect the {{ insert: param, sc-28_odp.01 }} of ...'), so every record that carries one also carries the same sentence with each placeholder resolved from the catalogue's own parameter labels and kept in square brackets — '[Selection (one or more): confidentiality; integrity]' — which is how NIST's own HTML rendering reads, and which is a sentence a person or a coding assistant can actually use. The verbatim text, placeholders and all, stays on the record as the evidence. SOC 2, ISO 27001 and PCI DSS are deliberately absent: that text is copyrighted and may not be republished.

**2,022 records.** Canonical, always-current version: [https://referencesource.org/security-compliance-controls/](https://referencesource.org/security-compliance-controls/)

| | |
|---|---|
| Last verified | 2026-11-15 |
| Re-check due | 2026-12-15 |
| Records | 2,022 |
| Machine-readable | [`data.json`](data.json) · [changes feed](https://referencesource.org/security-compliance-controls/changes.xml) |

Every record carries `source` (the page it came from) and `source_quote` (the exact line on that page which states it), so any value here can be checked without asking us. Where a source does not state something the row is omitted rather than guessed.

**Licence position for this dataset.** Both sources are US government works in the public domain: NIST SP 800-53 is published by NIST with its OSCAL rendering in a public GitHub repository, and the Code of Federal Regulations is published by the Office of the Federal Register. Each record links back to the exact API URL it was cut from and names the publisher's own page for the document. No text from SOC 2, ISO/IEC 27001 or PCI DSS appears anywhere in this dataset, because that text is copyrighted.

---

Snapshot of [referencesource.org](https://referencesource.org/security-compliance-controls/), which is canonical and re-verified on a schedule. If a record here is wrong, that is worth more to us than one that is right — please open an issue.
