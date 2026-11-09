# Awesome AI-Driven CRISPR Design 🧬🤖

[![Awesome]]
[![Update: Yearly]](#)
[![License: GPL v3]](LICENSE)
[![Paper](https://img.shields.io/badge/Preprint-Preprints.org-blue)](https://www.preprints.org/manuscript/202608.0824)

> **A curated, yearly-updated list of papers, tools, and datasets for AI-driven CRISPR-Cas system design.** 
> *Next scheduled update: 2027*

This repository serves as the official companion resource for our comprehensive review article: **"Evolution of AI-Driven CRISPR Systems: Tools, Methods, and Future Directions"** ([Preprints.org](https://www.preprints.org/manuscript/202608.0824)). 

Inspired by [papers_for_protein_design_using_DL], we categorize the tools into 8 functional modules (**C1–C8**) following the logical workflow of genome editing, bridging the gap between computational algorithms and wet-lab applications.

Contributions are warmly welcome! If you find a new paper or tool, please feel free to open a pull request or issue.

---

## 📑 Table of Contents
- [0. Benchmarks and Datasets](#0-benchmarks-and-datasets)
- [C1. CRISPR-Cas Database Search & Component Identification](#c1-crispr-cas-database-search--component-identification)
- [C2. CRISPR-Cas Structure Prediction](#c2-crispr-cas-structure-prediction)
- [C3. CRISPR-Cas Function Prediction](#c3-crispr-cas-function-prediction)
- [C4. CRISPR-Cas Sequence Generation](#c4-crispr-cas-sequence-generation)
- [C5. CRISPR-Cas Structure Generation](#c5-crispr-cas-structure-generation)
- [C6. Virtual Screening & Developability](#c6-virtual-screening--developability)
- [C7. DNA/RNA Synthesis Optimization](#c7-dnarna-synthesis-optimization)
- [C8. Gene Editing Experiment Design](#c8-gene-editing-experiment-design)
- [Highlight: Case Studies](#highlight-case-studies)
- [Recent Updates (Changelog)](#-recent-updates-changelog)

---

## 0. Benchmarks and Datasets

| Database / Resource | Description |
| :--- | :--- |
| [FLIP](#) | Benchmark tasks in fitness landscape inference for proteins |
| [ProteinGym](#) | Large-Scale Benchmarks for Protein Design and Fitness Prediction |
| [CRISPR-Cas Atlas](#) | Large-scale CRISPR operon datasets (used in OpenCRISPR-1) |
| [GUIDE-seq](#) | *In vivo* genome-wide unbiased identification of DSBs |
| [CHANGE-seq](#) | *In vitro* high-throughput analysis of nuclease genome-wide effects |
| [Detect-seq](#) | Reveals out-of-protospacer editing by base editors |

---

## C1. CRISPR-Cas Database Search & Component Identification

| Tool / Model | Description |
| :--- | :--- |
| [CRISPRCasFinder](#) | Identify and classify CRISPR-Cas systems and loci in genomes |
| [CRISPRminer](#) | Mining and annotation of CRISPR systems from (meta)genomes |
| [Protein2PAM](#) | Protein language model for PAM characterization |
| [DeepCRISPR](#) | Deep learning-based sgRNA design and off-target prediction |
| [CRISPOR](#) | sgRNA design, scoring, and off-target prediction (Cas9 etc.) |
| [TIGER](#) | Transformer-based model for Cas13d sgRNA design |
| [Elevation](#) | Machine learning model for comprehensive off-target assessment |
| [Cas-OFFinder](#) | Fast search algorithm for finding potential off-target sites |

---

## C2. CRISPR-Cas Structure Prediction

| Tool / Model | Description |
| :--- | :--- |
| [AlphaFold2](#) | Highly accurate single-chain protein structure prediction |
| [ESMFold](#) | Fast single-chain folding using protein language models |
| [AlphaFold3](#) | Multi-entity assembly and complex structure prediction |
| [RoseTTAFold All-Atom](#) | Multi-entity assembly including proteins, nucleic acids, and small molecules |
| [Chai-2](#) | Multimodal foundation model for biomolecular assembly |
| [ThermoMPNN](#) | Transfer learning model for predicting protein structure stability |

---

## C3. CRISPR-Cas Function Prediction

| Tool / Model | Description |
| :--- | :--- |
| [NucleicNet](#) | Deep learning model for predicting nucleic acid binding sites |
| [Metal3D](#) | 3D CNN for predicting metal ion binding sites |
| [SuperMetal](#) | Generative AI approach for metal ion binding site prediction |
| [DeepMVP](#) | Deep learning tool for post-translational modification (PTM) prediction |

---

## C4. CRISPR-Cas Sequence Generation

| Tool / Model | Description |
| :--- | :--- |
| [Evo](#) | Genomic language model for evolution-guided sequence generation |
| [ESM3](#) | Masked language model for function-to-sequence generation |
| [ProGen2](#) | Autoregressive LLM for protein sequence generation |
| [ProteinMPNN](#) | Message passing neural network for structure-to-sequence design |
| [LigandMPNN](#) | Context-conditioned neural network for structure-to-sequence design |

---

## C5. CRISPR-Cas Structure Generation

| Tool / Model | Description |
| :--- | :--- |
| [RFDiffusion](#) | SE(3) diffusion model for generative protein structure design |
| [Chroma](#) | Diffusion model for generative protein structure design |
| [BinderCraft](#) | Sequence-structure co-design using Diffusion and MPNN |
| [ProteinGenerator](#) | Sequence-structure co-design via sequence space diffusion |

---

## C6. Virtual Screening & Developability

| Tool / Model | Description |
| :--- | :--- |
| [EVOLVEpro](#) | PLM and active learning for predicting mutational effects |
| [AlphaMissense](#) | Deep learning model for predicting the effects of missense mutations |
| [LNP_ML](#) | Supervised machine learning for lipid nanoparticle (LNP) developability |
| [AGILE](#) | Deep learning platform for AAV developability and optimization |

---

## C7. DNA/RNA Synthesis Optimization

| Tool / Model | Description |
| :--- | :--- |
| [LinearDesign](#) | Computational linguistics approach for mRNA back translation and stability |
| [GEMORNA](#) | Deep generative model for RNA sequence optimization |

---

## C8. Gene Editing Experiment Design

| Tool / Model | Description |
| :--- | :--- |
| [CRISPR-GPT](#) | LLM agent for orchestrating the gene editing experiment design workflow |

---

## Highlight: Case Studies

Our review highlights three landmark cases where AI resolved long-standing bottlenecks in CRISPR engineering:

1. **Generative Design of Novel Nucleases:** [OpenCRISPR-1](#) (*Nature*, 2025) utilized PLMs to design a *de novo* editor with a 95% reduction in off-target activity compared to SpCas9.
2. **Structure-Informed Optimization:** Engineering compact Fanzor systems using AlphaFold3 and **EVOLVEpro** (*Nat Commun*, 2026) to fit within a single AAV vector.
3. **Predictive Modeling for Delivery:** Virtual screening of >40,000 ionizable lipids using machine learning (*Nat Mater*, 2024), accelerating LNP discovery from 18 months to under 6 months.

---

## 📅 Recent Updates (Changelog)

* **[2026.04]** 
  * Repository officially launched to accompany our review article on Preprints.org: [202608.0824](https://www.preprints.org/manuscript/202608.0824).
  * Initialized C1-C8 categorization and formatted tables.
  * Added foundational papers for CRISPR-Cas sequence generation (C4) and structure generation (C5).

---

## 🤝 Contributing

We welcome contributions! If you have a paper or tool that belongs on this list:
1. Fork the repository.
2. Add your entry to the appropriate `C1-C8` section using the table format.
3. Submit a Pull Request.

## 📝 Citation

If you find this repository useful for your research, please cite our review article:

Yang et al. Evolution of AI-Driven CRISPR Systems: Tools, Methods, and Future Directions. *Preprints* **2026**, 202608.0824. https://www.preprints.org/manuscript/202608.0824

```bibtex
@article{Yang2026AIDrivenCRISPR,
  author  = {Yang, Sam and others},
  title   = {Evolution of AI-Driven CRISPR Systems: Tools, Methods, and Future Directions},
  journal = {Preprints},
  year    = {2026},
  number  = {202608.0824},
  url     = {https://www.preprints.org/manuscript/202608.0824},
  note    = {Preprint}
}
```