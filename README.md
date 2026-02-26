# List of papers and tools about AI-driven CRISPR design

**AI 驱动 CRISPR 系统设计：论文与工具列表**

> This repository is inspired by [papers_for_protein_design_using_DL](https://github.com/Peldom/papers_for_protein_design_using_DL). We maintain a curated list of **papers and tools** on **AI-driven CRISPR–Cas design**, covering sgRNA design, off-target prediction, Cas discovery/engineering, structure prediction & generation, sequence design, delivery (LNP/AAV), and experiment planning. This list is maintained independently and **can be cited** as a companion resource; a detailed review article that references this repository may be published separately.
>
> Contributions and suggestions are warmly welcome!

_Papers / tools last week, updated on 2026.02.26:_

* Design of highly functional genome editors by modeling the universe of CRISPR-Cas sequences  
  * \[bioRxiv 2024.04.22.590591\] • \[code\]
* OpenCRISPR-1: de novo CRISPR-Cas design with protein language models  
  * \[Nature 2025\] • \[github\]
* Efficient generation of epitope-targeted de novo antibodies with Germinal  
  * \[bioRxiv 2025.09.19.677421\] • \[code\]
* Exploring the limits of pre-trained embeddings in machine-guided protein design: a case study on predicting AAV vector viability  
  * \[arXiv:2602.14828\] • \[code\]
* CasGen: A Regularized Generative Model for CRISPR Cas Protein Design  
  * \[bioRxiv 2025.02.28.640911\] • \[code\]

---

**AI for CRISPR design**

**0) Benchmarks and datasets**  
Sequence / screen datasets • Off-target assays • Databases • Similar lists • Guides  

**1) Reviews and surveys**  
AI–CRISPR overview • sgRNA design • Off-target • Cas engineering • Delivery & experiment design  

**2) Model-based design**  
Structure-prediction model-based (AlphaFold/ESM inversion) • LLM-based • Sampling algorithms  

**3) Function to scaffold**  
Diffusion-based • Flow-based • (Cas/scaffold backbone generation)  

**4) Scaffold to sequence**  
Inverse folding • Structure-to-sequence (ProteinMPNN, ESM-IF, LigandMPNN) • Train methods  

**5) Function to sequence**  
sgRNA/pegRNA design & efficiency • Off-target prediction • Sequence generation (pLM, diffusion) • RL-based  

**6) Function to structure**  
Cas structure generation • Sequence–structure co-design • Binder design  

**7) Other**  
Mutation / stability prediction • Delivery (LNP, AAV) • Experiment design • Similar lists  

---

## 0. Benchmarks and datasets

### 0.1 Sequence and screen datasets

**FLIP: Benchmark tasks in fitness landscape inference for proteins**  
Christian Dallago, Jody Mou, Kadina E Johnston, Bruce Wittmann, Nick Bhattacharya, Samuel Goldman, Ali Madani, Kevin K Yang  
NeurIPS 2021 Datasets and Benchmarks Track / bioRxiv 2021 • website • code • Supplementary  

**ProteinGym: Large-Scale Benchmarks for Protein Design and Fitness Prediction**  
Pascal Notin, Aaron W Kollasch, Daniel Ritter, et al.  
bioRxiv 2023.12.07.570727 • code  

**CRISPR–Cas Atlas (e.g. Profluent / OpenCRISPR)**  
Large-scale CRISPR operon datasets for training generative models  
• Ref: Ruffolo et al. Nature 2025  

### 0.2 Off-target and assay datasets

**GUIDE-seq**  
Genome-wide unbiased identification of DSBs enabled by sequencing  
Tsai et al. • in vivo off-target assay  

**CHANGE-seq**  
Circularization for high-throughput analysis of nuclease genome-wide effects by sequencing  
Lazzarotto et al. • in vitro • off-target data for model training  

**SITE-Seq**  
In vitro off-target profiling  

### 0.3 Databases

| Database / resource | Description |
|---------------------|-------------|
| [CRISPRCasFinder](https://crisprcas.i2bc.paris-saclay.fr/) | Identify and classify CRISPR-Cas systems and loci in genomes |
| [CRISPRCasdb](https://crisprcasdb.casbin.com/) | Comprehensive CRISPR-Cas database |
| [CRISPRminer](https://github.com/backmanlab/CRISPRminer) | Mining and annotation of CRISPR systems from (meta)genomes |
| [CRISPOR](http://crispor.tefor.net/) | sgRNA design, scoring, off-target prediction (Cas9 etc.) |
| [AlphaFoldDB](https://alphafold.ebi.ac.uk/) | Predicted protein structures (incl. Cas) |

### 0.4 Similar lists

* [papers_for_protein_design_using_DL](https://github.com/Peldom/papers_for_protein_design_using_DL) — Protein design with deep learning  
* [Machine-learning-for-proteins](https://github.com/kkahlhoff/Machine-learning-for-proteins) — Kevin K. Yang et al.  
* [awesome-AI-based-protein-design](https://github.com/topics/awesome-protein-design) — Protein design tools  

### 0.5 Guides

* CRISPOR documentation • CHOPCHOP • PrimeDesign  
* A review article citing this repository may be published separately (see above).  

---

## 1. Reviews and surveys

### 1.1 AI–CRISPR overview

**AI-driven CRISPR system design: tools, methods and perspectives**  
A detailed review that cites this repository as the curated list of papers and tools (five AI method categories, eight tool classes C1–C8, case studies, and outlook) may be published separately.  

**Design of highly functional genome editors by modeling the universe of CRISPR-Cas sequences**  
Jeffrey A. Ruffolo, Stephen Nayfach, Joseph Gallagher, Aadyot Bhatnagar, Joel Beazer, Riffat Hussain, Jordan Russ, Jennifer Yip, Emily Hill, Martin Pacesa, Alexander J. Meeske, Peter Cameron, Ali Madani  
bioRxiv 2024.04.22.590591 • code  

**Machine learning in CRISPR design**  
（综述类文献可在此持续补充）  

### 1.2 sgRNA design and efficiency

**Rule Set 2: Rational design of highly active sgRNAs for CRISPR-Cas9**  
Doench et al.  
Nat Biotechnol 2016 • on-target efficiency • RF-based  

**DeepCRISPR: predicting sgRNA on-target and off-target activity with deep learning**  
Chuai et al.  
Genome Biol 2018 • code • CNN, end-to-end  

**CRISPRon: a convolutional neural network for sgRNA on-target activity prediction**  
Nat Commun 2021 • multi-source data  

**TIGER: Cas13d gRNA design and on/off-target prediction**  
Nat Biotechnol 2023 • Cas13d  

**DeepCpf1 / Cas12a design**  
crRNA and efficiency prediction for Cpf1/Cas12a  

### 1.3 Off-target prediction

**CFD (Cutting Frequency Determination)**  
Gradient boosting / ML for off-target scoring  

**Elevation**  
Machine learning for off-target risk assessment  

**CRISPOR**  
Integrates multiple off-target algorithms  

**Cas-Offinder**  
Search for potential off-target sites  

### 1.4 Cas engineering and discovery

**OpenCRISPR-1: de novo design of CRISPR-Cas with protein language models**  
Ruffolo et al.  
Nature 2025 • ProGen2, CRISPR–Cas Atlas • github  

**EVOLVEpro: protein language model + few-shot active learning for enzyme design**  
Li et al. Nat Commun 2026 • AlphaFold3 + EVOLVEpro (Fanzor2) • code  

### 1.5 Delivery and experiment design

**LNP / AAV developability and ML**  
Li et al. Nat Mater 2024 (ionizable lipid discovery) • AGILE, COMET, MOSAIC, LNP_ML  

**CRISPR-GPT**  
Gene-editing experiment design from natural language  

---

## 2. Model-based design

> Inverting trained structure-prediction or generative models for design (e.g. “hallucination” for backbones).

### 2.1 Structure-prediction model-based (AlphaFold / ESM)

**De novo protein design by inversion of the AlphaFold structure prediction network**  
Casper Goverde, Benedict Wolf, Hamed Khakzad, Stephane Rosset, Bruno E Correia  
bioRxiv 2022.12.13.520346 • code  

**AlphaDesign: A de novo protein design framework based on AlphaFold**  
Jendrusch, Michael, Jan O. Korbel, S. Kashif Sadiq  
Mol Syst Biol 2025  

**Using AlphaFold for rapid and accurate fixed backbone protein design**  
Moffat, Lewis, Joe G. Greener, David T. Jones  
bioRxiv 2021  

**EvoBind: in silico directed evolution of peptide binders with AlphaFold**  
Patrick Bryant, Arne Elofsson  
bioRxiv 2022.07.23.501214 • code  

### 2.2 LLM-based

**Design of highly functional genome editors by modeling the universe of CRISPR-Cas sequences**  
Ruffolo et al.  
bioRxiv 2024.04.22.590591 • code • ProGen2, CRISPR-Cas Atlas  

**OpenCRISPR-1**  
Profluent AI • Nature 2025 • github  

### 2.3 Sampling algorithms

**AdaLead: adaptive greedy search for sequence design**  
Sam Sinai, Richard Wang, Alexander Whatley, et al.  
arXiv:2010.02141 (2020) • code  

**Plug & Play Directed Evolution with Gradient-based Discrete MCMC**  
Patrick Emami, Aidan Perreault, Jeffrey Law, et al.  
NeurIPS 2022 / arXiv:2212.09925  

---

## 3. Function to scaffold

> Backbone / scaffold generation (Cartesian, distance maps, angles). Conditional or unconditional generative models.

### 3.1 Diffusion-based

**RFDiffusion: de novo design of protein structure and function**  
Watson, Juergens, Bennett, et al.  
Nature 2023 • code • Colab  

**SE(3) diffusion model for protein backbone generation**  
Jason Yim, Brian L. Trippe, Valentin De Bortoli, et al.  
ICLR 2023 • code • Supplementary  

**Chroma**  
Generative structure design  

**RFDiffusionAA**  
All-atom generation  

### 3.2 Flow-based

**SE(3)-Stochastic Flow Matching for Protein Backbone Generation**  
Avishek Joey Bose, Tara Akhound-Sadegh, Kilian Fatras, et al.  
ICLR 2024  

**Fast protein backbone generation with SE(3) flow matching**  
Jason Yim, Andrew Campbell, et al.  
arXiv:2310.05297 • code  

**Proteina: Scaling Flow-based Protein Structure Generative Models**  
Tomas Geffner, Kieran Didi, et al.  
ICLR 2025 Oral • code • website  

---

## 4. Scaffold to sequence

> Inverse folding: sequence from backbone/scaffold (torsion, distances, atoms). Includes rotamer recovery.

### 4.0 Review

**Protein sequence design on given backbones with deep learning**  
Yufeng Liu, Haiyan Liu  
Protein Eng Des Sel 2023  

**Generative AI for Controllable Protein Sequence Design: A Survey**  
Yiheng Zhu, Zitai Kong, Jialu Wu, et al.  
arXiv:2402.10516  

### 4.1 Inverse folding (structure-to-sequence)

**Robust deep learning based protein sequence design using ProteinMPNN**  
Justas Dauparas, Ivan Anishchenko, Nathaniel Bennett, et al.  
Science 2022 • code • hugging face • lecture • colab  

**PiFold: Toward effective and efficient protein inverse folding**  
Zhangyang Gao, Cheng Tan, Stan Z. Li  
ICLR 2023 • github  

**ESM-IF (Inverse Folding)**  
Learning inverse folding from millions of predicted structures  
Chloe Hsu, Robert Verkuil, Jason Liu, et al. • bioRxiv 2022  

**LigandMPNN**  
Atomic context-conditioned protein sequence design  
Justas Dauparas, Gyu Rie Lee, et al.  
Nat Methods 2025 • code  

**Knowledge-Design: Pushing the limit of protein design via knowledge refinement**  
Zhangyang Gao, Cheng Tan, Stan Z. Li  
ICLR • code  

---

## 5. Function to sequence

> Generate or score sequences from desired function (e.g. efficiency, specificity, stability).

### 5.1 Traditional supervised / RF

**Rule Set 2**  
Doench et al. Nat Biotechnol 2016 • RF, on-target sgRNA efficiency  

**CFD, Elevation**  
Off-target scoring (gradient boosting / ML)  

### 5.2 Deep learning (CNN, RNN, DNN)

**DeepCRISPR**  
Chuai et al. Genome Biol 2018 • CNN, off-target prediction • code  

**BE-Hive**  
Deep learning for base editor efficiency and window  

**FORECasT, Lindel**  
Indel / repair outcome prediction (DNN/CNN)  

### 5.3 Attention / Transformer

**CRISPRon**  
Nat Commun 2021 • multi-source, cross-dataset  

**DTMP-Prime**  
pegRNA activity (prime editing)  

**CRISP-RCNN**  
Cas9 multi-task (on/off-target)  

**TIGER**  
Cas13d gRNA design and on/off-target  
Nat Biotechnol 2023  

### 5.4 Generative (pLM, diffusion, VAE)

**ProGen2, ESM2, ESM3**  
Protein language models for Cas representation and sequence generation  

**OpenCRISPR-1**  
Ruffolo et al. Nature 2025 • ProGen2 fine-tuned for CRISPR–Cas • github  

**Protein design with guided discrete diffusion**  
Nate Gruver, Samuel Stanton, Nathan C. Frey, et al.  
NeurIPS 2024 • code • lecture  

**CasGen: A Regularized Generative Model for CRISPR Cas Protein Design**  
Bharani Nammi, et al.  
bioRxiv 2025.02.28.640911 • code  

### 5.5 RL-based

**Model-based reinforcement learning for biological sequence design**  
Christof Angermueller, David Dohan, et al.  
ICLR 2019  

**Self-play reinforcement learning guides protein engineering**  
Yi Wang, Hui Tang, et al.  
Nat Mach Intell 2023 • code  

（CRISPR 场景下 gRNA 文库设计、LNP 配方优化等 RL 工作可在此持续补充）  

---

## 6. Function to structure

> Generate structure from function or recover partial structure (inpainting). Includes sequence–structure co-design.

### 6.0 Review

**Towards deep learning sequence-structure co-generation for protein design**  
Chentong Wang, Sarah Alamdari, et al.  
Curr Opin Struct Biol 2025  

### 6.1 Diffusion-based

**RFDiffusion**  
Watson et al. Nature 2023 • code • Colab  

**De novo design of high-affinity protein binders with AlphaProteo**  
DeepMind • arXiv:2409.08022  

**BinderCraft: one-shot design of functional protein binders**  
Martin Pacesa, Lennart Nickel, et al.  
Nature 2025 • code  

**RFDiffusion3**  
De novo design of all-atom biomolecular interactions  
Baker lab • bioRxiv 2025.09.18.676967 • code  

### 6.2 AlphaFold / RoseTTAFold-based

**Generalized Biomolecular Modeling and Design with RoseTTAFold All-Atom**  
Rohith Krishna, Jue Wang, Woody Ahern, et al.  
Science • code  

**AlphaFold3**  
All-atom, multi-entity (protein–nucleic acid–small molecule)  
DeepMind  

**RF-AllAtom, BOLTZ-2, Chai-2**  
All-atom complex prediction (Cas–gRNA–DNA 等)  

### 6.3 Flow-based

**ProteinZen: combining latent and SE(3) flow matching for all-atom protein generation**  
Alex Li, Tanja Kortemme  
NeurIPS 2024 ML4SB  

**FlowDesign: Improved Design of Antibody CDRs Through Flow Matching**  
Jun Wu, Xiangzhe Kong, et al.  
Cell Systems 2025 • code  

---

## 7. Other

### 7.1 Mutation / stability / fitness

**AlphaMissense**  
Proteome-wide missense variant effect prediction  
Cheng et al. Science • code • data  

**Rapid protein stability prediction using deep learning representations**  
Lasse M Blaabjerg, Maher M Kassem, et al.  
eLife 2023 • code  

**EVOLVEpro**  
Protein language model + few-shot active learning for enzyme design  
Li et al. Nat Commun 2026 • used in Fanzor2 engineering  

### 7.2 Delivery (LNP, AAV)

**Machine learning and combinatorial chemistry for ionizable lipid discovery (LNP)**  
Li et al. Nat Mater 2024 • 119-23 lipid • code (Suppl.)  

**AGILE**  
AAV / delivery developability  
Nat Commun 2024  

**COMET, MOSAIC, LNP_ML**  
Developability assessment for LNP / AAV  

### 7.3 Experiment design and assistants

**CRISPR-GPT**  
Gene-editing experiment design from natural language  

### 7.4 Similar lists and resources

* [papers_for_protein_design_using_DL](https://github.com/Peldom/papers_for_protein_design_using_DL) — Protein design with deep learning  
* [OpenCRISPR](https://github.com/Profluent-AI/OpenCRISPR) — OpenCRISPR-1 sequences and release (license for commercial/therapeutic use)  
* A review article that uses this list (methods, tables, case studies, challenges) may be published separately and will cite this repo.  

---

## About

List of papers and tools about **AI-driven CRISPR design**.

### Topics

crispr • deep-learning • sgRNA-design • off-target • gene-editing • protein-design

### Resources

* [README](README.md)  
* [Contributing](CONTRIBUTING.md)  

### License

[GPL-3.0](LICENSE)

### How to cite

If you use this list in your work, please cite this repository (e.g. GitHub URL or Zenodo DOI if you add one). A detailed review article that references this repo may be published separately.

*Last updated: 2026.02.26*
