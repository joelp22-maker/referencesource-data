# Kubernetes component version skew policy: how far apart component versions can be in a supported cluster

The maximum version difference Kubernetes supports between cluster components, one record per governed component pair (kube-apiserver to kubelet, kube-proxy, kubectl, and the kube-controller-manager/kube-scheduler/cloud-controller-manager group, plus the kube-apiserver-to-kube-apiserver HA rule and the kube-proxy-to-kubelet rule), from the project's own version-skew-policy page. Answers 'how many minor versions behind can my kubelet be', 'can kubectl be newer than kube-apiserver', 'what must already be upgraded before I upgrade this component'. Getting this wrong during a rolling upgrade breaks node registration or blocks the upgrade path, usually discovered mid-rollout. The rule text is stable in structure release to release; the version numbers in the worked examples move with each Kubernetes minor release, so the numeric examples need re-verification on that cadence.

**6 records.** Canonical, always-current version: [https://referencesource.org/kubernetes-version-skew-policy/](https://referencesource.org/kubernetes-version-skew-policy/)

| | |
|---|---|
| Last verified | 2026-09-02 |
| Re-check due | 2026-12-30 |
| Records | 6 |
| Machine-readable | [`data.json`](data.json) · [changes feed](https://referencesource.org/kubernetes-version-skew-policy/changes.xml) |

Every record carries `source` (the page it came from) and `source_quote` (the exact line on that page which states it), so any value here can be checked without asking us. Where a source does not state something the row is omitted rather than guessed.

**Licence position for this dataset.** Source is the Kubernetes project's own documentation (kubernetes.io), a CNCF project. The page footer reads 'Documentation Distributed under CC BY 4.0'. We take the fact plus a short attributed quote linking back.

---

Snapshot of [referencesource.org](https://referencesource.org/kubernetes-version-skew-policy/), which is canonical and re-verified on a schedule. If a record here is wrong, that is worth more to us than one that is right — please open an issue.
