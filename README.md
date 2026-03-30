## In this repository, we provide essential files for a manuscript: "De_novo_design_of_KRas4B-G12D_miniprotein_inhibitor"

#### Simulating packages used in this work for conducting MD simulations:

##### gromacs/2023.3 and gromacs/2025.2-plumed-2.10.0-gcc-nvhpcx packages were used to perform conventional MD and Well-tempered MetaDynamcis simulation, respectively. Both utilize the CHARMM36m force field.

# Highlights from this work:




```
####python -m pip install sklearn
```

**More details:**

1. Initial systems used to conduct MD simulations are stored in Folder: **0-initial-systems**
2. Results of Principle Components Analysis (PCA) of the standard MD productions runs cna be found in the Folder: **1-PCA_analysis_6000ns_standard_MD**, together with the notebook script for performing PCA.
3. Essential files for performing the Well-tempered MetaDynamcis simulation are shown in file: **2-files_of_Well_tempered_MetaD-5600ns**, the related results will be presented in the manuscript.
4. HADDOCK2.4 was used to perform the docking analysis and the corresponding results are provided in Folder: **3-Docking_analysis**.
5. Final equilibrated structures of the complexes of pepide-KRas (G12D and wild-type) in its two nucleotide states, obtained from 500 ns molecular dynamics simulations for each system. Binding energies of peptide and KRas of all systems considered in this work using MMPBSA are provided in the **4-binding_selectivity**.
