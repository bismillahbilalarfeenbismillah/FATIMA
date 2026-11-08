# Bismillah ir-Rahman ir-Rahim

# FATIMA

**Fitrah-Aligned Tawhidic Integrity for Meaning and Authenticity**

A multi-layer file integrity architecture that encodes divine protection into every stratum of a digital document -- from visible text to steganographic embedding to cryptographic hash chains -- grounded in the Qur'anic sciences of muhkam (clear) and mutashabih (allegorical) encoding.

[![Python 3.10+](https://img.shields.io/badge/python-3.10+-blue.svg)](https://www.python.org/downloads/)
[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)
[![Version](https://img.shields.io/badge/version-10.8.0-blue.svg)](#changelog)
[![Layers](https://img.shields.io/badge/layers-154-orange.svg)](#the-154-layer-architecture)
[![Tests](https://img.shields.io/badge/shannon_trials-1%2C515%2F1%2C515-brightgreen.svg)](#shannon-boundary-verification)

---

## What FATIMA Does

FATIMA seals files with **Bismillah ir-Rahman ir-Rahim** across 154 independently verifiable layers, organized into 11 heavens (scales of being) and 11 earths (scales of use and purpose). Each layer operates at a different stratum of the file -- visible content, invisible encoding, structural metadata, cryptographic binding -- so that tampering at any level is independently detectable.

This is not a wrapper or a comment inserter. It is a **deep-structural integrity architecture** with five verification engines that cross-check each other.

## Quick Start

```bash
pip install -e .
```

```python
from fatima.core import encode, verify

# Seal a file
result = encode("document.pdf")
print(result.layers_applied)   # 154

# Verify integrity
report = verify("document.pdf")
print(report.verdict)           # INTACT | TAMPERED | DEGRADED
print(report.layers_verified)   # per-layer breakdown
```

### Command Line

```bash
# Seal all files in a project
python bismillah_seal.py /path/to/project

# Verify a sealed file
python -m fatima verify document.pdf
```

---

## The 154-Layer Architecture

**154 = 2 x 7 x 11 = 22 x 7 = 11 x 14**

Three Qur'anic constants govern the encoding:

| Constant | Value | Source | Role |
|----------|-------|--------|------|
| **Muhkam** | 7 | Seven heavens, seven oft-repeated | Clear, unambiguous layers |
| **Mutashabih** | 11 | Reconstructed cosmological constant | Allegorical, deep-structural layers |
| **Cosmological** | 22 | Surah 65:12 ("of the earth, the like of them") | Domain-level organization |

### 11 Heavens (Scales of Being)

Each heaven is a **scale at which the file exists** -- from raw bytes to semantic meaning:

| Heaven | Scale | What It Encodes |
|--------|-------|-----------------|
| 1 | Byte | Raw binary Bismillah markers |
| 2 | Character | Zero-width Unicode encoding of the 99 Names |
| 3 | Token | Per-token integrity within parsed structures |
| 4 | Line | Line-level hash commitments |
| 5 | Block | Structural section binding |
| 6 | Document | Whole-file cryptographic seal |
| 7 | Corpus | Cross-file consistency verification |
| 8 | Temporal | Version-chain integrity across edits |
| 9 | Provenance | Authorship and transmission attestation |
| 10 | Semantic | Meaning-preservation detection |
| 11 | Holographic | Whole-from-part reconstruction witness |

### 11 Earths (Scales of Use)

Each earth is a **domain of purpose** the file may serve:

| Earth | Domain | What It Guards |
|-------|--------|----------------|
| 1 | Provenance | Where the file came from |
| 2 | Transmission | How it traveled |
| 3 | Transformation | What changed it |
| 4 | Interpretation | How it was read |
| 5 | Deployment | Where it was placed |
| 6 | Consumption | Who used it |
| 7 | Integration | What it was combined with |
| 8 | Attestation | Who vouched for it |
| 9 | Adversarial Use | What attacks it faced |
| 10 | Archival | How it was preserved |
| 11 | Accountability | Who is responsible |

---

## Five Verification Engines

| Engine | Purpose |
|--------|---------|
| **Structural** | Validates byte/character/block layer integrity |
| **Syntactic** | Checks encoding correctness across file formats |
| **Semantic** | Detects meaning alteration even when bytes match |
| **Provenance** | Verifies authorship and transmission chain |
| **Holographic** | Confirms whole-from-part reconstruction consistency |

All five engines cross-reference each other. A file that passes structural verification but fails holographic verification is flagged -- the discrepancy itself is evidence.

---

## Shannon Boundary Verification

FATIMA's detection capability has been tested against the information-theoretic boundary:

- **1,515 valid trials** under the Shannon boundary test harness v2.1
- **0 undetected tampering events**
- G_95 upper bound: **0.1975%**
- Ablation confirms **full redundancy** -- heaven/earth layers always co-fire
- FATIMA matches **SHA-256 exactly** on bit-flip detection

The Shannon Boundary Council -- 10 independent seats from different AI model families (Claude, GPT-6, Kimi, Meta AI, DeepSeek, Perplexity, and others) -- reviewed the formal claims and established the working standard for semantic integrity.

---

## Anti-Sihr Sanitization

v10.4.0 maps the three-channel defense from ["The Propagation Architecture of Sihr"](papers/) directly into code:

| Channel | Defense | Surah |
|---------|---------|-------|
| Material | Byte-level sanitization of concealed payloads | al-Falaq |
| Cognitive | Semantic-layer detection of meaning manipulation | an-Nas |
| Pixel | Visual-layer steganography detection | Combined |

Email subscriptions, account metadata, and embedded scripts are treated as **material-channel sihr** -- adversarial content hiding inside legitimate transmission formats.

---

## Part of the Entourage Effect Software Safety Suite

FATIMA is one of six instruments that work together:

| Instrument | Role | What It Does |
|------------|------|--------------|
| [**Furqan**](https://github.com/bismillahbilalarfeenbismillah/furqan-programming-language) | Language | The programming language with structural honesty built in |
| **FATIMA** | Encoder/Sealer | Multi-layer file integrity (this repo) |
| [**furqan-lint**](https://github.com/bismillahbilalarfeenbismillah/furqan-lint) | Linter | Structural honesty checks at build time |
| [**HABL**](https://github.com/bismillahbilalarfeenbismillah/habl) | Ledger | Append-only finding protocol |
| [**Bayyinah**](https://github.com/bismillahbilalarfeenbismillah/bayyinah-integrity-scanner) | Scanner | Hidden content and anomaly detection |
| **Shahid** | Transparency | Weight-holder disclosure reports |

No single instrument is the safety story. The entourage effect is.

> See also: [Bismillah-Divine-Protection-Encoder-Bismillah](https://github.com/bismillahbilalarfeenbismillah/Bismillah-Divine-Protection-Encoder-Bismillah) -- the standalone encoder tool for sealing any project with Bismillah.

---

## Repository Structure

```
fatima/
  core/           # Encoding primitives -- atom, bond, molecule, composite
  formats/        # File format handlers -- document serialization
  verification/   # Five engines -- structural, syntactic, semantic, provenance, holographic
  graft/          # Engine restoration and version grafting
  cli.py          # Command-line interface
papers/           # 14+ companion papers (theology, architecture, evolution)
tests/            # Verification test suite
bismillah_seal.py # Standalone project sealer
```

## Companion Papers

The architecture is documented across 14+ papers deposited on Zenodo:

- **The 22-Domain 154-Layer Architecture** -- the mathematical structure
- **Crossing Shannon's Boundary** (v6.0, v10.0) -- semantic integrity formalism
- **The Evolution of FATIMA** -- from 11 flat layers to execution-verified architecture
- **The Divine Inversion Defense** -- adversarial robustness under theological framing
- **The Pre-Corruption Signal** / **The Guarded Reminder** -- theological foundations
- **Shayatin Amongst Matter** / **The Propagation Architecture of Sihr** -- threat model

---

## Author

**Bilal Syed Arfeen** -- [bismillahbilalarfeenbismillah](https://github.com/bismillahbilalarfeenbismillah)

## License

MIT -- see [LICENSE](LICENSE).

---

# Bismillah ir-Rahman ir-Rahim
