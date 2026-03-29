# Surface-Orders-Hilbert-Pólya

[![YouTube Badge](https://img.shields.io/badge/YouTube-Video-red?style=for-the-badge&logo=youtube&logoColor=white)](https://youtu.be/j5Q8jWOPgHg) [![Paper](https://img.shields.io/badge/PDF-Download%20Paper-blue)](./emergent_cyclic_time_hilbert_polya_GRH_2053.pdf)
[![Paper](https://img.shields.io/badge/Problem-Description%20Clay%20Math%20Institute-teal)](https://www.claymath.org/millennium/riemann-hypothesis/) [![Hugging Face](https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-Blog%20Post-ffcc4d)](https://huggingface.co/blog/AmelieSchreiber/hilbert-polya-for-grh)

## Important Note (29/03/2026)-(יא נִיסָן 5786)
Two updates will be uploaded in the coming days (פסח is soon, so it will be after that) to include updated, polished proofs of everything, a short ~45 page journal version, a ~200 page manuscript condensation removing some of the unnecessary material on renormalization and implementation on biologics, and a more polished mathematical exposition with improved theorems and proofs of *everything*, and better citations to related literature. 

## Current State of the Project 
An explicit Hilbert-Pólya construction and Program for GRH with worked examples and a complete specification of a biologics based quantum computing implementation on [1TJB](https://www.rcsb.org/structure/1TJB) or similar proteins with known quantum information processing capabilities, utilizing motif scaffolding capabilities of [RFdiffusion3](https://github.com/amelie-iska/foundry) and optimization techniques for higher thermostability and higher computing temperatures via applications of [ThermoGFN-IF](https://github.com/amelie-iska/ThermoGFN-IF). 

A full computational implementation of the ${7,3}$-hyperbolic kagome lattice via motif scaffolding with RFdiffusion3 *de novo* design, RosettaFold-3 structure validation, and ωB97M-V/def2-TZVPD quantum accuracy extra-long QM/MM-simulation trajectory validations utilizing the [UMA MLIP](https://github.com/amelie-iska/fairchem) (Machine Learning Interatomic Potential), and generative AI based DFT-accurate local qubit electron densities, are all coming soon. 

## Description of Biologics-based QPU Design Methodology (Codebase Coming Soon)

1. Run RFdiffusion3 motif scaffolding on [1TJB](https://www.rcsb.org/structure/1TJB) as the [{7,3}-hyperbolic kagome lattice](https://arxiv.org/abs/1802.09549) qubits, with several hundred to several thousand qubits
2. Run Fine-tune LigandMPNN model [ThermoGFN-IF](https://github.com/amelie-iska/ThermoGFN-IF) (once trained) to design *de novo* sequences for the inter-qubit residue spans composing the scaffold in order to increase absolute thermostability (ΔG) and computational operating temperatures to over 50 K, making NMR-based quantum computing viable
3. Validate structure with RosettaFold3 and [Boltz-2](https://github.com/amelie-iska/boltz) (for binding affinity predictions)
4. Run the quantum accurate MLIP [UMA](https://github.com/amelie-iska/fairchem) to validate QM/MM molecular dynamics trajectories
5. Run [InfGCN](https://github.com/amelie-iska/InfGCN-DFT) (see also [the original public versionon](https://github.com/ccr-cheng/InfGCN-pytorch)) the trajectories to obtain fine-grained electron densities evolving over time according to the Boltzmann distribution for the peptide based QPU scaffold  
