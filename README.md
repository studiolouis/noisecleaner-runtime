# noisecleaner-runtime

Runtime component packs for **NoiseCleaner** (a Windows tool by
Studio Louis that removes noise from audio/video files locally with
DeepFilterNet).

NoiseCleaner's DL edition does not bundle its heavy third-party
runtime. On first launch the app downloads the pack from this
repository's Releases, verifies it against a SHA-256 pinned in the
app, and extracts it next to the executable. After that one download
the app works fully offline.

## Contents

The pack contains **only open-source libraries**, redistributed under
their respective licenses:

- PyTorch 2.8.0 / torchaudio 2.8.0 (BSD-style license)
- DeepFilterNet 0.5.6 (MIT / Apache-2.0)
- PyAV 14.2.0 (BSD)
- NumPy 1.26.4 (BSD)
- …and their dependencies (loguru, sympy, networkx, etc.)

It contains **no** Studio Louis source code and **no** model weights
(the DeepFilterNet2 weights are fetched separately from the official
DeepFilterNet repository by the app).

## Releases

- `v1` — `noisecleaner-runtime-v1.zip` (147,885,889 bytes)
  SHA-256: `49b116f9ef90a2097a42eb4454d0fdaaccb815cadb52cd6f42ee3a1a0aa5e9fe`
