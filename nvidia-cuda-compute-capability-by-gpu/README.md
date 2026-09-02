# NVIDIA GPU CUDA compute capability by model

Which CUDA compute capability version (e.g. '8.9', '12.0') each NVIDIA GPU model supports, from NVIDIA's own compute-capability table. Compute capability determines which CUDA toolkit version a card needs, which `-arch=sm_XX` / `-gencode` build flags to pass (the target is the capability written without its dot, so 8.9 is sm_89 and 12.0 is sm_120), and whether a PyTorch/TensorFlow wheel built for one architecture will run on a given card. Answers 'what compute capability is my GPU', 'does CUDA 11.8 support the RTX 4090', 'what sm_XX target do I use for an A100'. NVIDIA's own page is the single source of truth and is already well-ranked for individual current-generation cards; the value here is completeness (legacy cards back to the earliest Fermi/Kepler-era GPUs, and every SKU in a generation, not just the flagship) in one machine-readable table, and being current the moment a new architecture (e.g. Blackwell, 12.x) ships, before third-party blogs catch up.

**441 records.** Canonical, always-current version: [https://referencesource.org/nvidia-cuda-compute-capability-by-gpu/](https://referencesource.org/nvidia-cuda-compute-capability-by-gpu/)

| | |
|---|---|
| Last verified | 2026-09-01 |
| Re-check due | 2026-12-26 |
| Records | 441 |
| Machine-readable | [`data.json`](data.json) · [changes feed](https://referencesource.org/nvidia-cuda-compute-capability-by-gpu/changes.xml) |

Every record carries `source` (the page it came from) and `source_quote` (the exact line on that page which states it), so any value here can be checked without asking us. Where a source does not state something the row is omitted rather than guessed.

**Licence position for this dataset.** Source is NVIDIA's own developer documentation (developer.nvidia.com). We take the fact (model to compute-capability mapping) plus attribution linking back; we do not reproduce NVIDIA's full page design or unrelated content.

---

Snapshot of [referencesource.org](https://referencesource.org/nvidia-cuda-compute-capability-by-gpu/), which is canonical and re-verified on a schedule. If a record here is wrong, that is worth more to us than one that is right — please open an issue.
