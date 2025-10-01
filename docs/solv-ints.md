---
hide:
  - navigation
---

# Supported Solvents and Initiators

---

## Supported Solvents

---

Updating this list is more involved. Please write me if you would like a new initiator or solvent added.

| Solvent                                | Acronym                |    Smiles   |
| ------------------                     | -------                |  ---------  |
| Water                                  |   SPC                  |             |
| Acetonitrile                           |   MeCN                 | CC#N        |
| Chloroform                             |   CHL                  | C(Cl)(Cl)Cl |
| Dimethylformamide                      |   DMF                  | CN(C)C=O    |
| Dimethyl Sulfoxide                     |   DMSO                 | CS(=O)C     |

Solvent parameters are hard-coded, and are not derived from ACPYPE for each run like the functional monomers. VirualChemistry.org entries are available [here](https://virtualchemistry.org/ff.php) and are originally from [Caleman et al.](https://doi.org/10.1021/ct200731v). A combination are used, with new atom types supplied for Caleman's molecules.

| Solvent Acronym |   Target Density (kg/mol)  | Acpype GAS | Acpype BCC | VirtualChemistry.Org |
| ----------------| ---------------   | ---------  | ---------  | ------ |
|       CHL       |       1489        |  1365 (-8%)| 1371 (-8%) |<b> 1466 (-2%) </b>|
|       DMF       |       944         |  955 (1%) | <b> 957 (1%) </b> | 924 (-2%) |
|      DMSO       |       1100        |  1095 (0%)| <b> 1096 (0%) </b>| 1115 (1%) |
|      MeCN       |       786         |  723 (-8%)|  726 (-8%) |<b> 789 (0%) </b>|

---

## Supported Initiators

---

| Initiator                              | Acronym                |    Smiles   |
| ------------------                     | -------                |  ---------  |
| Ammonium Persulfate                    |   APS                  | \[NH4+\].O=S(=O)(\[O-\])[O] |
| 4,4'-Azobis(4-cyanopentanoic Acid)     |   ACPA                 | C\[C\](CCC(O)=O)C#N with N#N|
| Azobisisobutyronitrile                 |   AIBN                 | C=CC(=O)N with N#N|
| Tetramethylethylenediamine             |   TEMED/TMEDA/TMD      | N(CCN(C)C)(C)C        |

<!-- | Functional Monomers to Add             | Acronym | Vina | MIPkit - V |    Smiles   |
| ------------------                     | ------- |      |       |  ---------  |
|                              |         |      |       |          |
|                              |         |      |       |          |
|                              |         |      |       |          |
|                              |         |      |       |          |
|                                        |         |      |       |          |
|                                        |         |      |       |          |
|                                        |         |      |       |          | -->