## In this repository, we provide essential files for a manuscript: "Structure-guided De Novo Design of a Selective Miniprotein Inhibitor for KRas4B-G12D."

#### Simulating packages used in this work for conducting MD simulations:

##### gromacs/2023.3 and gromacs/2025.2-plumed-2.10.0-gcc-nvhpcx packages were used to perform conventional MD and Well-tempered MetaDynamcis simulation, respectively. Both utilize the CHARMM36m force field.

# Highlights from this work:




```
####python -m pip install sklearn
```

**More details:**

1. Initial systems used to conduct MD simulations are stored in Folder: **0-initial-systems**
2. Results of Principle Components Analysis (PCA) of the standard MD productions runs, totalling 6000 ns, can be found in the Folder: **1-PCA_analysis_6000ns_standard_MD**, together with the notebook script (pca-md.ipynb) for performing PCA.
3. Essential files for performing the Well-tempered MetaDynamcis simulation are shown in file: **2-files_of_Well_tempered_MetaD-5600ns**, the related results will be presented in the manuscript.
4. HADDOCK2.4 was used to perform the docking analysis and the corresponding results are provided in Folder: **3-Docking_analysis**. Eight structures of the complexes of pepide-KRas (G12D and wild-type) solvated in NaCl aq. of 150 mM in two different nucleotide states (GTP-bound and GDP-bound). The final equilibrated complex of KRas-miniprotein after running 1000 ns molecular dynamics simulations for each system are also presented in their corresponding folders. 
5. Binding energies of peptide and KRas of all systems considered in this work using MMPBSA are provided in the **4-binding_selectivity**.
