## In this repository, we provide essential files for a manuscript: "Structure-Guided Design of a c-Src-Inspired Miniprotein Inhibitor Targeting KRas4B-G12D."

by Huixia Lu*, Jordi Faraudo, and Jordi Marti

#### Simulating packages used in this work for conducting MD simulations:

##### gromacs/2023.3 and gromacs/2025.2-plumed-2.10.0-gcc-nvhpcx packages were used to perform conventional MD and Well-tempered MetaDynamcis simulation, respectively. Both utilize the CHARMM36m force field.

# Highlights from this work:

- Enhanced sampling identifies two distinct low-energy conformational states (A and C) of the 41-residue KRas-targeting miniprotein.
- Miniprotein state A exhibits preferential binding to KRas4B-G12D over wild-type KRas4B, independent of nucleotide-bound state.
- Differential KRas recognition is primarily mediated by interactions with the switch regions rather than direct contacts with the G12D mutation site.
- The miniprotein N-terminal region (residues 1-23) plays a key role in stabilizing the G12D-associated binding interface.
- Mutation-induced changes in the KRas conformational landscape promote an indirect, ensemble-mediated mechanism of miniprotein recognition.

**More details:**

1. Initial systems used to conduct MD simulations are stored in Folder: **0-initial-systems**
2. Results of Principle Components Analysis (PCA) of the standard MD productions runs, totalling 6000 ns, can be found in the Folder: **1-PCA_analysis_6000ns_standard_MD**, together with the notebook script (pca-md.ipynb) for performing PCA.
3. Essential files for performing the Well-tempered MetaDynamcis simulation are shown in file: **2-files_of_Well_tempered_MetaD-5600ns**, the related results will be presented in the manuscript.
4. HADDOCK2.4 was used to perform the docking analysis and the corresponding results are provided in Folder: **3-Docking_analysis**. 8 MD systems across mutation + nucleotide states were subsequently considered to extract quantitative and mechanistically consistent metrics in this section [Eight structures of the complexes of pepide-KRas (G12D and wild-type) solvated in NaCl aq. of 150 mM in two different nucleotide states (GTP-bound and GDP-bound)]. The final equilibrated complex of KRas-miniprotein after running 1000 ns molecular dynamics simulations for each system are also presented in their corresponding folders. 
5. The last 500ns of production run of each system was used for calculating the binding energies of peptide and KRas using *gmx_MMPBSA*. An example set of input files for the G12D-mutated KRas4B–GTP system in complex with state A of the miniprotein, prepared for the gmx_MMPBSA method, is provided in the **4-binding_selectivity** directory. And the corresponding results of binding energies across eight systems are shown here:

![binding.png](https://github.com/HuixiaLuScienceRocks/De_novo_design_of_KRas4B-G12D_miniprotein_inhibitor/blob/main/4-binding_selectivity/binding.png)
