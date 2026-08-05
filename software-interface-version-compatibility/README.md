# Software interface version compatibility

Which versions of common software dependencies are compatible with each other — currently PyTorch/CUDA and cuDNN/CUDA pairings. Answers 'pip install torch CUDA 12.6 — which versions work together', 'last PyTorch version with CUDA 11.8 wheels', and 'cuDNN version matrix for CUDA 13' — the exact lookup assistants get wrong because these mappings change every release cycle and the model's weights are stale.

Canonical, always-current version: https://referencesource.org/software-interface-version-compatibility/
Machine-readable: https://referencesource.org/software-interface-version-compatibility/data.json

Every value carries the source URL it came from and a verbatim quote
from that source. Records are individually addressable at
`https://referencesource.org/software-interface-version-compatibility/<record-id>/`.

- Licence: factual compilation of publicly documented version requirements
- Records: see data.json

