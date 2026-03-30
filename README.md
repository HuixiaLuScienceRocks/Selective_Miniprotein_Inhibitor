## In this repository, we provide essential files for a manuscript: "De_novo_design_of_KRas4B-G12D_miniprotein_inhibitor"

#### Simulating packages used in this work for conducting MD simulations:

##### gromacs/2023.3 and gromacs/2025.2-plumed-2.10.0-gcc-nvhpcx packages were used to perform conventional MD and Well-tempered MetaDynamcis simulation, respectively. Both utilize the CHARMM36m force field.

# Highlights from this work:




```
####python -m pip install sklearn
```

**More details:**

1. Initial systems used to conduct MD simulations are stored in Folder: **0-initial-systems**
2. In the Folder: **toy_data** you will find an example of aaa.txt which is part of the data set I have used to construct MSMs for system KRas4B-G12D-GTP (paper in preparation). I couldn't upload the whole data because of the size limit.
3. A walk through tutorial of how to construct MSMs is shown in file: **msm-analysis.ipynb**
4. PDB files of KRas4B-GTP and KRas4B-GDP were extracted from Macrostates by PyEMMA after constructing MSMs, the corresponding results are installed in Folders: **kras4b-g12d-gtp and kras4b-g12d-gdp**.
5. Final equilibrated structures of complex of Src-KRas in its two nucleotide states, obtained from 200 ns molecular dynamics simulations performed with NAMD and initialized from HADDOCK2.4 docking results for KRas-Src macrostates with HADDOCK scores above 130, are provided in the **HADDOCK_results folder**.
