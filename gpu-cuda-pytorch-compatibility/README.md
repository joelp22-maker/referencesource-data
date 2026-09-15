# PyTorch release, CUDA build and NVIDIA driver pairings

One record per (PyTorch release, CUDA build) pairing: which CUDA builds each PyTorch release ships wheels for, which Python versions it supports, which cuDNN it carries, which GPU architectures (compute capabilities) the wheel was compiled for, and the minimum NVIDIA driver the pairing needs. Answers 'does torch 2.7 run on an RTX 5090', 'nvidia-smi says CUDA 12.4 but torch wants 12.6 — do I need a new driver', 'which pip index URL do I use for CUDA 12.8', 'why is torch.cuda.is_available() False on a card that CUDA supports'. Nobody publishes this join: PyTorch's release notes state the CUDA builds but not the driver floor, NVIDIA's release notes state the driver floor but say nothing about PyTorch, and the compiled architecture list lives only in PyTorch's own build script. The pairing is what a person actually needs and it is the thing assistants get wrong.

**45 records.** Canonical, always-current version: [https://referencesource.org/gpu-cuda-pytorch-compatibility/](https://referencesource.org/gpu-cuda-pytorch-compatibility/)

| | |
|---|---|
| Last verified | 2026-09-14 |
| Re-check due | 2026-12-13 |
| Records | 45 |
| Machine-readable | [`data.json`](data.json) · [changes feed](https://referencesource.org/gpu-cuda-pytorch-compatibility/changes.xml) |

Every record carries `source` (the page it came from) and `source_quote` (the exact line on that page which states it), so any value here can be checked without asking us. Where a source does not state something the row is omitted rather than guessed.

**Licence position for this dataset.** PyTorch's RELEASE.md and build scripts are BSD-3-Clause (pytorch/pytorch LICENSE); NVIDIA's CUDA release notes are vendor technical documentation. We take facts (version pairings, driver floors, architecture lists) plus a short attributed quote linking back to each source. We do not reproduce either document.

---

Snapshot of [referencesource.org](https://referencesource.org/gpu-cuda-pytorch-compatibility/), which is canonical and re-verified on a schedule. If a record here is wrong, that is worth more to us than one that is right — please open an issue.
