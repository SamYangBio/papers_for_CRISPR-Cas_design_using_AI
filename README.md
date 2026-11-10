# Awesome AI-Driven CRISPR Design 🧬🤖

[![Awesome]]
[![Update: Yearly]](#)
[![License: GPL v3]](LICENSE)
[![Paper](https://img.shields.io/badge/Preprint-Preprints.org-blue)](https://www.preprints.org/manuscript/202608.0824)

> **A curated, yearly-updated list of papers, tools, and datasets for AI-driven CRISPR-Cas system design.** 
> *Next scheduled update: 2027*

This repository serves as the official companion resource for our comprehensive review article: **"AI-Driven CRISPR Design: Methods, Tools, Applications and Challenges"** ([Preprints.org](https://www.preprints.org/manuscript/202608.0824)). 

Inspired by [papers_for_protein_design_using_DL](https://github.com/Peldom/papers_for_protein_design_using_DL), we categorize the tools into 8 functional modules (**C1–C8**) following the logical workflow of genome editing, bridging the gap between computational algorithms and wet-lab applications.

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
| [FLIP](https://doi.org/10.1101/2021.11.09.467890) | Benchmark tasks in fitness landscape inference for proteins |
| [ProteinGym](https://doi.org/10.1101/2023.12.07.570727) | Large-Scale Benchmarks for Protein Design and Fitness Prediction |
| [CRISPR-Cas Atlas](https://github.com/Profluent-AI/CRISPR-Cas-Atlas) | Large-scale CRISPR operon datasets (used in OpenCRISPR-1) |
| [GUIDE-seq](https://doi.org/10.1038/nbt.3117) | *In vivo* genome-wide unbiased identification of DSBs |
| [CHANGE-seq](https://doi.org/10.1038/s41587-020-0555-7) | *In vitro* high-throughput analysis of nuclease genome-wide effects |
| [Detect-seq](https://doi.org/10.1038/s41592-021-01172-w) | Reveals out-of-protospacer editing by base editors |

---

## C1. CRISPR-Cas Database Search & Component Identification

| Tool / Model | Description |
| :--- | :--- |
| [CRISPRCasFinder](https://doi.org/10.1093/nar/gky425) | Identify and classify CRISPR-Cas systems and loci in genomes |
| [CRISPRminer](https://doi.org/10.1038/s42003-018-0184-6) | Mining and annotation of CRISPR systems from (meta)genomes |
| [Protein2PAM](https://doi.org/10.1038/s41587-025-02995-0) | Protein language model for PAM characterization |
| [DeepCRISPR](https://doi.org/10.1186/s13059-018-1459-4) | Deep learning-based sgRNA design and off-target prediction |
| [CRISPOR](https://doi.org/10.1093/nar/gkw360) | sgRNA design, scoring, and off-target prediction (Cas9 etc.) |
| [TIGER](https://doi.org/10.1038/s41587-023-01830-8) | Transformer-based model for Cas13d sgRNA design |
| [Elevation](https://doi.org/10.1038/nbt.4061) | Machine learning model for comprehensive off-target assessment |
| [Cas-OFFinder](https://doi.org/10.1093/bioinformatics/bts573) | Fast search algorithm for finding potential off-target sites |

---

## C2. CRISPR-Cas Structure Prediction

| Tool / Model | Description |
| :--- | :--- |
| [AlphaFold2](https://doi.org/10.1038/s41586-021-03819-2) | Highly accurate single-chain protein structure prediction |
| [ESMFold](https://doi.org/10.1126/science.ade2574) | Fast single-chain folding using protein language models |
| [AlphaFold3](https://doi.org/10.1038/s41586-024-07487-w) | Multi-entity assembly and complex structure prediction |
| [RoseTTAFold All-Atom](https://doi.org/10.1126/science.adl2528) | Multi-entity assembly including proteins, nucleic acids, and small molecules |
| [Chai-2](https://www.chaidiscovery.com/) | Multimodal foundation model for biomolecular assembly |
| [ThermoMPNN](https://doi.org/10.1073/pnas.2314828121) | Transfer learning model for predicting protein structure stability |

---

## C3. CRISPR-Cas Function Prediction

| Tool / Model | Description |
| :--- | :--- |
| [NucleicNet](https://doi.org/10.1038/s41467-019-12920-0) | Deep learning model for predicting nucleic acid binding sites |
| [Metal3D](https://doi.org/10.1038/s41467-023-37870-6) | 3D CNN for predicting metal ion binding sites |
| [SuperMetal](https://doi.org/10.1186/s13321-025-01038-9) | Generative AI approach for metal ion binding site prediction |
| [DeepMVP](https://doi.org/10.1038/s41592-025-02797-x) | Deep learning tool for post-translational modification (PTM) prediction |

---

## C4. CRISPR-Cas Sequence Generation

| Tool / Model | Description |
| :--- | :--- |
| [Evo](https://doi.org/10.1126/science.ado9336) | Genomic language model for evolution-guided sequence generation |
| [ESM3](https://doi.org/10.1126/science.ads0018) | Masked language model for function-to-sequence generation |
| [ProGen2](https://doi.org/10.1016/j.cels.2023.10.002) | Autoregressive LLM for protein sequence generation |
| [ProteinMPNN](https://doi.org/10.1126/science.add2187) | Message passing neural network for structure-to-sequence design |
| [LigandMPNN](https://doi.org/10.1038/s41592-025-02626-1) | Context-conditioned neural network for structure-to-sequence design |

---

## C5. CRISPR-Cas Structure Generation

| Tool / Model | Description |
| :--- | :--- |
| [RFdiffusion](https://doi.org/10.1038/s41586-023-06415-8) | SE(3) diffusion model for generative protein structure design |
| [Chroma](https://doi.org/10.1038/s41586-023-06728-8) | Diffusion model for generative protein structure design |
| [BindCraft](https://doi.org/10.1038/s41586-025-09446-5) | Sequence-structure co-design using Diffusion and MPNN |
| [ProteinGenerator](https://doi.org/10.1038/s41587-024-02160-z) | Sequence-structure co-design via sequence space diffusion |

---

## C6. Virtual Screening & Developability

| Tool / Model | Description |
| :--- | :--- |
| [EVOLVEpro](https://doi.org/10.1126/science.adr6006) | PLM and active learning for predicting mutational effects |
| [AlphaMissense](https://doi.org/10.1126/science.adg7492) | Deep learning model for predicting the effects of missense mutations |
| [LNP_ML](https://doi.org/10.1038/s41563-024-01867-3) | Supervised machine learning for lipid nanoparticle (LNP) developability |
| [AGILE](https://doi.org/10.1038/s41467-024-50673-5) | Deep learning platform for LNP developability and optimization |

---

## C7. DNA/RNA Synthesis Optimization

| Tool / Model | Description |
| :--- | :--- |
| [LinearDesign](https://doi.org/10.1038/s41586-023-06127-z) | Computational linguistics approach for mRNA back translation and stability |
| [GEMORNA](https://doi.org/10.1016/j.jpha.2026.101671) | Deep generative model for RNA sequence optimization |

---

## C8. Gene Editing Experiment Design

| Tool / Model | Description |
| :--- | :--- |
| [CRISPR-GPT](https://doi.org/10.1038/s41551-025-01463-z) | LLM agent for orchestrating the gene editing experiment design workflow |

---

## Highlight: Case Studies

Our review highlights three landmark cases where AI resolved long-standing bottlenecks in CRISPR engineering:

1. **Generative Design of Novel Nucleases:** [OpenCRISPR-1](https://doi.org/10.1038/s41586-025-09298-z) (*Nature*, 2025) utilized PLMs to design a *de novo* editor with a 95% reduction in off-target activity compared to SpCas9. ([GitHub](https://github.com/Profluent-AI/OpenCRISPR))
2. **Structure-Informed Optimization:** Engineering compact Fanzor systems using [AlphaFold3](https://doi.org/10.1038/s41586-024-07487-w) and [EVOLVEpro](https://doi.org/10.1126/science.adr6006) (*[Nat Commun](https://doi.org/10.1038/s41467-026-68644-5)*, 2026) to fit within a single AAV vector.
3. **Predictive Modeling for Delivery:** Virtual screening of >40,000 ionizable lipids using machine learning (*[Nat Mater](https://doi.org/10.1038/s41563-024-01867-3)*, 2024), accelerating LNP discovery from 18 months to under 6 months.

---

## 📅 Recent Updates (Changelog)

* **[2026.04]** 
  * Repository officially launched to accompany our review article on Preprints.org: [202608.0824](https://www.preprints.org/manuscript/202608.0824).
  * Initialized C1-C8 categorization and formatted tables.
  * Added foundational papers for CRISPR-Cas sequence generation (C4) and structure generation (C5).
* **[2026.11]** 
  * Added primary paper / resource links (DOI or official page) for tools and datasets in C1–C8 and case studies.

---

## 🤝 Contributing

We welcome contributions! If you have a paper or tool that belongs on this list:
1. Fork the repository.
2. Add your entry to the appropriate `C1-C8` section using the table format.
3. Submit a Pull Request.

## 📝 Citation

If you find this repository useful for your research, please cite our review article:

Zheng-xia Yang. AI-Driven CRISPR Design: Methods, Tools, Applications and Challenges. *Preprints* **2026**, 202608.0824. https://www.preprints.org/manuscript/202608.0824

```bibtex
@article{Yang2026AIDrivenCRISPR,
  author  = {Zheng-xia Yang},
  title   = {AI-Driven CRISPR Design: Methods, Tools, Applications and Challenges},
  journal = {Preprints},
  year    = {2026},
  number  = {202608.0824},
  url     = {https://www.preprints.org/manuscript/202608.0824},
  note    = {Preprint}
}
```
