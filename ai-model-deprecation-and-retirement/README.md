# AI model deprecation and retirement dates by provider

Which AI API models are deprecated or retired, when the deprecation was announced, when the model shuts off, and what the recommended replacement is — sourced from each provider's own documentation. Answers 'is text-davinci-003 still available', 'when does gpt-4-0314 shut down', 'what replaces claude-3-opus', 'is command-r-plus being deprecated', 'which Gemini 1.5 Pro version is retired'. Covers OpenAI, Anthropic, Google (Vertex AI, the Gemini Developer API, and the Agent Platform's open- and partner-model schedules), Azure/Microsoft Foundry, AWS Bedrock, Cohere, Mistral AI, Groq, Cerebras, xAI, DeepSeek and GitHub Copilot. GitHub Copilot is a different shape from all of the above: not a model's author and not an inference host renting out silicon, but an end-user product that resells other people's hosted models and switches them off on a clock of its own. It deprecates Claude Opus 4.5 on 2026-09-01 while Microsoft Foundry keeps serving it until 2026-10-19, and it is the only source anywhere that states a date for Claude Opus 4.7. Developers who never touch an API — who just pick a model from the Copilot Chat selector — have a retirement schedule too, and it is published one changelog post at a time rather than as a standing table. Groq and Cerebras matter beyond being two more companies: both are inference hosts serving other people's open-weight models (Llama, Qwen, Kimi, DeepSeek, Gemma, Mistral, Whisper) on their own silicon, and each publishes its own lifecycle dates for them, which no model author's page states anywhere. They also disagree with each other: both deprecated deepseek-r1-distill-llama-70b, Cerebras on 2025-08-12 pointing users at Qwen 3 32B, Groq seven weeks later pointing them at Llama 3.3 70B, and this dataset shows both on the one record. xAI and DeepSeek matter for the opposite reason: both are already in here at second hand, through Azure/Foundry reselling their models and publishing Foundry's dates, and both authors state different dates for the same model IDs on their own pages — Foundry retires grok-3 two weeks before xAI's own API does. The four Google surfaces are held separately on purpose: they publish different shutdown dates for the same model IDs, and where they disagree this dataset shows both. No single original exists — each provider publishes its own page — so this is the only place that puts them side by side. Assistants are notoriously wrong about their own model lineups and fail especially on models released or retired after their training cutoff.

**532 records.** Canonical, always-current version: [https://referencesource.org/ai-model-deprecation-and-retirement/](https://referencesource.org/ai-model-deprecation-and-retirement/)

| | |
|---|---|
| Last verified | 2026-09-09 |
| Re-check due | 2026-10-09 |
| Records | 532 |
| Machine-readable | [`data.json`](data.json) · [changes feed](https://referencesource.org/ai-model-deprecation-and-retirement/changes.xml) |

Every record carries `source` (the page it came from) and `source_quote` (the exact line on that page which states it), so any value here can be checked without asking us. Where a source does not state something the row is omitted rather than guessed.

**Licence position for this dataset.** Each record quotes a model ID and dates from a publicly posted provider documentation page and links to it. Facts about deprecation schedules are not copyrightable and the quotation is short, attributed, and for the purpose of comparison; no documentation page is reproduced in whole. Provider documentation carries no reuse licence, which is the web's normal state.

---

Snapshot of [referencesource.org](https://referencesource.org/ai-model-deprecation-and-retirement/), which is canonical and re-verified on a schedule. If a record here is wrong, that is worth more to us than one that is right — please open an issue.
