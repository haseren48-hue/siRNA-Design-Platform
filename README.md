# siRNA-Design-Platform
An automated, genome-wide specific siRNA design tool optimized for in vitro transcription.

# siRNA Design & Off-Target Profiling Platform

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/haseren48-hue/siRNA-Design-Platform/blob/main/siRNA_Design_Platform.ipynb)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

An automated, genome-wide specific siRNA design and off-target profiling pipeline optimized for T7 *in vitro* transcription (IVT). 

## 🌟 Key Features
- **Efficacy Guaranteed:** Applies strict thermodynamic guidelines for highly effective siRNA selection.
- **High Specificity:** Prevents seed-dependent off-target effects by strictly evaluating the melting temperature (Tm ≤ 21.5°C) of the seed region using the Nearest-Neighbor method.
- **Genome-wide Profiling:** Automates BLAST+ searches against mammalian genomes (via Google Drive or NCBI Datasets) to rigorously filter out potential off-targets.
- **Common Target Mode:** Capable of identifying conserved siRNA sequences across multiple gene variants or species.
- **Ready for IVT Synthesis:** Automatically generates order-ready DNA template sequences with customizable T7 promoters and 5' extensions.
- **Zero Environment Setup:** Fully executable in the browser via Google Colab.

## 🚀 Pipeline Overview
This tool guides you through 5 simple steps:
1. **Target Discovery:** Input your sequence (single or multiple) to find candidates meeting the design criteria.
2. **Genome Database Setup:** Mount your custom genome (`.fna`) or download directly from NCBI.
3. **Off-target Profiling:** Strict screening using `blastn-short` to evaluate off-target risks.
4. **Template Generation:** Output clean, order-ready CSV files for DNA oligo synthesis.

## 📖 Citations & Algorithms
This pipeline evaluates siRNA candidates based on the established thermodynamic rules:
- **Efficacy:** Ui-Tei, K. et al., *Nucleic Acids Res* 32, 936-948 (2004).
- **Specificity:** Ui-Tei, K. et al., *Nucleic Acids Res* 36, 7100-7109 (2008).

## 👤 Author
**Fumiya Hasegawa, DVM**
