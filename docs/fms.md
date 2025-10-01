---
hide:
  - navigation
---

# Supported Functional Monomers

---

The following list is a range of functional monomers found in literature. Not all (like those containing Boron or Silicon) will be supported by all softwares.

Supplementing this list is easy, as all are found in `./constants/fm_list.yaml`. If you do modify this list, make sure to reinitialize MIPkit to rebuild the .sdf files for docking and the .yaml encoding file for polymerization. Make sure to follow the commented directions in the yaml file, or else you will break backwards compatibility.

| Functional Monomer                     | Acronym                | Vina    | gnina    | MIPkit (vi) |    Smiles   |
| ------------------                     | -------                | ------- | -------  | ------- |  ---------  |
| Acrylic Acid                           |   AAC                  |&#x2611; |&#x2611;  |&#x2611; | C=CC(=O)O |
| Acrylamide                             |   AAM                  |&#x2611; |&#x2611;  |&#x2611; | C=CC(=O)N |
| 4-Acryloylmorpholine                   |  ACMO                  |&#x2611; |&#x2611;  |&#x2611; | C=CC(=O)N1CCOCC1 |
| Acrylonitrile                          |   ACN                  |&#x2611; |&#x2611;  |&#x2611; | C=CC#N |
| Acrolein                               |  ACRO                  |&#x2611; |&#x2611;  |&#x2611; | C=CC=O |
| Aminoethyl methacrylate                |  AEMA                  |&#x2611; |&#x2611;  |&#x2611; | CC(=C)C(=O)OCCN |
| Aminoethyl methacrylamide              |  AEMAA                 |&#x2611; |&#x2611;  |&#x2611; | N(CCN)C(=O)C(=C)C |
| Allylamine                             |  ALLY                  |&#x2611; |&#x2611;  |&#x2611; | C=CCN |
| Allylpiperazine                        |  ALPP                  |&#x2611; |&#x2611;  |&#x2611; | C=CCN1CCNCC1 |
| Acrylamido Methyl Propanesulfonic Acid |  AMPSA                 |&#x2611; |&#x2611;  |&#x2611; | CC(C)(CS(=O)(=O)O)NC(=O)C=C |
| Aminopropyl methacrylamide             |  APMA                  |&#x2611; |&#x2611;  |&#x2611; | CC(=C)C(=O)NCCCN |
| Aminopropyltriethoxysilane             |  APTES                 |&#x2611; |&#x2611;  |         | CCO\[Si\](CCCN)(OCC)OCC |
| Allylthiourea                          |  AT                    |&#x2611; |&#x2611;  |&#x2611; | C=CCNC(=S)N |
| p-Aminostyrene                         |  p-AS                  |&#x2611; |&#x2611;  |&#x2611; | C=CC1=CC=C(C=C1)N |
| Butyl acrylate                         |  BA                    |&#x2611; |&#x2611;  |&#x2611; | CCCCOC(=O)C=C |
| Butyl Methacrylate                     |  BMA                   |&#x2611; |&#x2611;  |&#x2611; | CCCCOC(=O)C(=C)C |
| Benzyl Methacrylate                    |  BZMA                  |&#x2611; |&#x2611;  |&#x2611; | CC(=C)C(=O)OCC1=CC=CC=C1 |
| Carboxybetaine Methacrylate            | CBMA                   |&#x2611; |&#x2611;  |&#x2611; | O=C(CC\[N+\](C)(C)CCOC(C(C)=C)=O)\[O-\] |
| Diallyl methylamine                    | DAMAS                  |&#x2611; |&#x2611;  |&#x2611; | CN(CC=C)CC=C |
| 2-(Diethylamino)ethyl acrylate         | DEAA                   |&#x2611; |&#x2611;  |&#x2611; | CCN(CC)CCOC(=O)C=C |
| Diethylamino ethyl methacrylate        | DEAEMA                 |&#x2611; |&#x2611;  |&#x2611; | CCN(CC)CCOC(=O)C(C)=C |
| Diethylene Glycol Dimethacrylate       | DEGDMA                 |&#x2611; |&#x2611;  |&#x2611; | CC(=C)C(=O)OCCOCCOC(=O)C(=C)C |
| N,N-Dimethylacrylamide                 | DMAA                   |&#x2611; |&#x2611;  |&#x2611; |  CN(C)C(=O)C=C |
| Dimethylamino ethyl methacrylate       | DMAEMA                 |&#x2611; |&#x2611;  |&#x2611; | CC(=C)C(=O)OCCN(C)C |
| Dimethylamino propyl methacrylamide    | DMAPMAA                |&#x2611; |&#x2611;  |&#x2611; | CN(C)CCCNC(=O)C(C)=C |
| Ethylene glycol dicyclopentenyl ether acrylate    |  EGDPEA     |&#x2611; |&#x2611;  |&#x2611; | C=CC(=O)OCCOC1CC2CC1C3C=CCC23 |
| Ethylene glycol methacylate phosphate  |  EGMP                  |&#x2611; |&#x2611;  |&#x2611; | CC(=C)C(=O)OCCOP(O)(O)=O |
| Ethylene glycol methyl ether methacrylate | EGMEM               |&#x2611; |&#x2611;  |&#x2611; | COCCOC(=O)C(C)=C |
| Ethylene glycol phenyl ether acrylate     | EGPEA               |&#x2611; |&#x2611;  |&#x2611; | C=CC(=O)OCCOc1ccccc1 |
| 2-Ethylstyrene                         |  2-ES                  |&#x2611; |&#x2611;  |&#x2611; | CCC1=CC=CC=C1C=C |
| 4-Ethylstyrene                         |  4-ES                  |&#x2611; |&#x2611;  |&#x2611; | CCC1=CC=C(C=C1)C=C |
| 2-Formylphenylboronic acid             | 2-FPBA                 |         |&#x2611;  |         | B(C1=CC=CC=C1C=O)(O)O |
| 3-Formylphenylboronic acid             | 3-FPBA                 |         |&#x2611;  |         | B(C1=CC(=CC=C1)C=O)(O)O |
| 4-Formylphenylboronic acid             | 4-FPBA                 |         |&#x2611;  |         | B(C1=CC=C(C=C1)C=O)(O)O |
| Furfuryl methacrylate                  |  FFMA                  |&#x2611; |&#x2611;  |&#x2611; | CC(=C)C(=O)OCc1ccco1 |
| Glycidyl methacrylate                  |   GMA                  |&#x2611; |&#x2611;  |&#x2611; | CC(=C)C(=O)OCC1CO1 |
| 2-Hydroxyethyl Acrylate                |  HEA                   |&#x2611; |&#x2611;  |&#x2611; | C=CC(=O)OCCO |
| Hydroxyethyl acrylamide                |  HEAA                  |&#x2611; |&#x2611;  |&#x2611; | C=CC(=O)NCCO |
| Hydroxyethyl methacrylate              |  HEMA                  |&#x2611; |&#x2611;  |&#x2611; | CC(=C)C(=O)OCCO |
| Hydroxypropyl methacrylamide           |  HPMA                  |&#x2611; |&#x2611;  |&#x2611; | CC(=C)C(=O)NCCCO |
| Isobutyltriethoxysilane                |  IPTS                  |&#x2611; |&#x2611;  |         | CCO\[Si\](CC(C)C)(OCC)OCC |
| Isobutyl acrylate                      |   IBA                  |&#x2611; |&#x2611;  |&#x2611; | CC(C)COC(=O)C=C |
| Isobutyl methacrylate                  |   IBMA                 |&#x2611; |&#x2611;  |&#x2611; | CC(C)COC(=O)C(C)=C |
| Itaconic Acid                          |    IA                  |&#x2611; |&#x2611;  |&#x2611; | C=C(CC(=O)O)C(=O)O |
| Methacrylic Acid                       |   MAA                  |&#x2611; |&#x2611;  |&#x2611; | CC(=C)C(=O)O |
| Methacryloyl L-aspartic acid           |  MALAA                 |&#x2611; |&#x2611;  |&#x2611; | CC(=C)C(=O)N\[C@@H\](CC(=O)O)C(=O)O |
| Methacylic acid N-hydroxysyccinimide ester   |  MAHSE           |&#x2611; |&#x2611;  |&#x2611; | CC(=C)C(=O)ON1C(=O)CCC1=O |
| N,N,N-trimethyl-3-\[(2-methylacryloyl)amino\]propan-1-aminium |  MAPTAC  |&#x2611; |&#x2611;  |&#x2611; | CC(=C)C(=O)NCCC\[N+\](C)(C)C |
| Methacrylamide                         |   MAM                  |&#x2611; |&#x2611;  |&#x2611; | CC(=C)C(=O)N |
| 4-Methacryloxyethyl trimellitic anhydride  |  4-META            |&#x2611; |&#x2611;  |&#x2611; | O1C(=O)c2c(ccc(c2)C(=O)OCCOC(=O)C(=C)C)C1=O |
| \[2-(Methacryloyloxy)ethyl\]trimethylammonium | METC            |&#x2611; |&#x2611;  |&#x2611; | CC(=C)C(=O)OCC\[N+\](C)(C)C |
| 2-Methacryloyloxyethyl phosphorylcholine | MPC                  |&#x2611; |&#x2611;  |&#x2611; | CC(=C)C(=O)OCCOP(=O)(\[O-\])OCC\[N+\](C)(C)C |
| 4-Methylstyrene                        |  4-MS                  |&#x2611; |&#x2611;  |&#x2611; | CC1=CC=C(C=C1)C=C |
| Methylacryloxyprolyl Trimethoxysilane  |  MPTS                  |&#x2611; |&#x2611;  |         | CO\[Si\](CCCOC(=O)C(C)=C)(OC)OC |
| Methyl 2-acetamidoacrylate             |  MAAA                  |&#x2611; |&#x2611;  |&#x2611; | COC(=O)C(=C)NC(C)=O |
| Methyl methacrylate                    |   MMA                  |&#x2611; |&#x2611;  |&#x2611; | CC(=C)C(=O)OC |
| N-Isopropylacrylamide                  |  NIPAM                 |&#x2611; |&#x2611;  |&#x2611; | CC(C)NC(=O)C=C |
| N-(4-Ethenylphenyl)-N'-methylthiourea  |   NMT                  | &#x2611; |&#x2611; |&#x2611; | CNC(=S)NC1=CC=C(C=C1)C=C |
| N-Phenylacrylamide                     |   NPA                  |&#x2611; |&#x2611;  |&#x2611; | C=CC(=O)NC1=CC=CC=C1 |
| Phenyl Acrylamide                      |   PAM                  |&#x2611; |&#x2611;  |&#x2611; | C=C(C1=CC=CC=C1)C(=O)N |
| Phenyl methacrylate                    |   PMA                  |&#x2611; |&#x2611;  |&#x2611; | CC(=C)C(=O)Oc1ccccc1 |
| Propyl methacrylate                    |   PPMA                 |&#x2611; |&#x2611;  |&#x2611; | CCCOC(=O)C(C)=C |
| Pyrrole                                |  PY                    |&#x2611; |&#x2611;  |&#x2611; | C1=CNC=C1 |
| 4-Vinylphenol                          |  PVP                   |&#x2611; |&#x2611;  |&#x2611; | C=CC1=CC=C(C=C1)O |
| Sulfobetaine Methacrylate              |  SBMA                  |&#x2611; |&#x2611;  |&#x2611; | CC(=C)C(=O)OCC\[N+\](C)(C)CCCS(=O)(=O)O |
| Phenylethene (Styrene)                 |  STYR                  |&#x2611; |&#x2611;  |&#x2611; | C=CC1=CC=CC=C1 |
| N-tert-Butylacrylamide                 |   TBA                  |&#x2611; |&#x2611;  |&#x2611; | CC(C)(C)NC(=O)C=C |
| 1-(4-Vinylphenyl)-3-(3,5-bis(trifluoromethyl)phenyl)urea | TBFM |&#x2611; |&#x2611;  |&#x2611; | C=CC1=CC=C(C=C1)NC(=O)NC2=CC(=CC(=C2)C(F)(F)F)C(F)(F)F |
| Trifluoromethacrylic Acid              |  TFMAA                 |&#x2611; |&#x2611;  |&#x2611; | C=C(C(=O)O)C(F)(F)F |
| Urocanic Acid                          |   UCA                  |&#x2611; |&#x2611;  |         | C1=C(NC=N1)/C=C/C(=O)O |
| Urocanic Acid Ethyl Ester              |  UCAEE                 |&#x2611; |&#x2611;  |         | CCOC(=O)/C=C/C1=CN=CN1 |
| p-Vinylbenzoic Acid                    |  p-VBA                 |&#x2611; |&#x2611;  |&#x2611; | C=CC1=CC=C(C=C1)C(=O)O |
| Vinylbenzyl Chloride                   |  VBC                   |&#x2611; |&#x2611;  |&#x2611; | C=CC1=CC=C(C=C1)CCl |
| 9-Vinylcarbazole                       |  9-VC                  |&#x2611; |&#x2611;  |&#x2611; | C=Cn1c2ccccc2c3ccccc13 |
| N-Vinylcaprolactam                     |  NVCL                  |&#x2611; |&#x2611;  |&#x2611; | C=CN1CCCCCC1=O |
| N-Vinylformamide                       |  NVF                   |&#x2611; |&#x2611;  |&#x2611; | C=CNC=O |
| 1-vinylimidazole                       |  1-VI                  |&#x2611; |&#x2611;  |&#x2611; | C=CN1C=CN=C1 |
| 4,5-vinylimidazole                     |  45-VI                 |&#x2611; |&#x2611;  |&#x2611; | C=CC=1NC=NC1 |
| 4-Vinylbenzlamine                      |  VNA                   |&#x2611; |&#x2611;  |&#x2611; | C=CC1=CC=C(C=C1)CN |
| 2-vinylpyridine                        |  2-VP                  |&#x2611; |&#x2611;  |&#x2611; | C=CC1=CC=CC=N1 |
| 4-vinylpyridine                        |  4-VP                  |&#x2611; |&#x2611;  |&#x2611; | C=CC1=CC=NC=C1 |
| Vinylphosphonic Acid                   |   VPA                  |&#x2611; |&#x2611;  |&#x2611; | C=CP(=O)(O)O |
| 2-vinylphenylboronic acid              | 2-VPBA                 |         |&#x2611;  |         | B(C1=CC=CC=C1C=C)(O)O |
| 3-vinylphenylboronic acid              | 3-VPBA                 |         |&#x2611;  |         | B(C1=CC(=CC=C1)C=C)(O)O |
| 4-vinylphenylboronic acid              | 4-VPBA                 |         |&#x2611;  |         | B(C1=CC=C(C=C1)C=C)(O)O |
| Vinyl pyrrolidone                      |   VPD                  |&#x2611; |&#x2611;  |&#x2611; | C=CN1CCCC1=O |

| Cross-linker                           | Acronym                | Vina    | gnina    | MIPkit |    Smiles   |
| ------------------                     | -------                |         | -------   |  ---------  | ------- |
| Allyl Methacrylate                     |   AMA                  |&#x2611; |&#x2611;  |&#x2611; | CC(=C)C(=O)OCC=C |
| Bis(acrylamido)pyridine                |  BAAPy                 |&#x2611; |&#x2611;  |&#x2611; | C=CC(=O)NC1=NC(=CC=C1)NC(=O)C=C |
| 1,4-Bis(acryloyl)piperazine            |   BAPA                  |&#x2611; |&#x2611;  |&#x2611; | C=CC(=O)N1CCN(CC1)C(=O)C=C |
| Methylenebisacrylamide                 |   BIS                  |&#x2611; |&#x2611;  |&#x2611; | C=CC(=O)NCNC(=O)C=C |
| Diallyl Carbonate                      |   DAC                  |&#x2611; |&#x2611;  |&#x2611; | C=CCOC(=O)OCC=C |
| 1,3-Diisopropoylbenzene                |  DIPB                  |&#x2611; |&#x2611;  |&#x2611; | CC(=C)C1=CC(=CC=C1)C(=C)C |
| m-Divinylbenzene                       |  m-DVB                 |&#x2611; |&#x2611;  |&#x2611; | C=CC1=CC(C=C)=CC=C1 |
| o-Divinylbenzene                       |  o-DVB                 |&#x2611; |&#x2611;  |&#x2611; | C=CC1=C(C=C)C=CC=C1 |
| p-Divinylbenzene                       |  p-DVB                 |&#x2611; |&#x2611;  |&#x2611; | C=CC1=CC=C(C=C)C=C1 |
| Ethylenebisacrylamide                  |  EBAM                  |&#x2611; |&#x2611;  |&#x2611; | C=CC(=O)NCCNC(=O)C=C |
| Ethylene glycol dimethacrylate         |  EGDMA                 |&#x2611; |&#x2611;  |&#x2611; | CC(=C)C(=O)OCCOC(=O)C(=C)C |
| 2-(methacryloyloxy)ethyl phosphate     |   MEP                  |&#x2611; |&#x2611;  |&#x2611; | CC(=C)C(=O)OCCOP(O)(=O)OCCOC(=O)C(C)=C |
| N,O-Bismethacryloyl ethanolamine       |  NOBE                  |&#x2611; |&#x2611;  |&#x2611; | CC(=C)C(=O)NCCOC(=O)C(=C)C |
| 1,4-Phenylene dimethacrylate           |  PDMA                  |&#x2611; |&#x2611;  |&#x2611; | CC(=C)C(=O)Oc1ccc(OC(=O)C(C)=C)cc1 |
| Pentaerythritol triacrylate            |  PE3A                  |&#x2611; |&#x2611;  |&#x2611; | C=CC(=O)OCC(CO)(COC(=O)C=C)COC(=O)C=C         |
| Pentaerythritol tetraacrylate          |  PE4A                  |&#x2611; |&#x2611;  |&#x2611; | C=CC(=O)OCC(COC(=O)C=C)(COC(=O)C=C)COC(=O)C=C |
| Tetraoxysilane                         |  TEOS                  |&#x2611; |&#x2611;  |         | \[H\]\[Si\](OCC)(OCC)OCC |
| Trimethylolpropane dimethacrylate      |  TMPD                  |&#x2611; |&#x2611;  |&#x2611; | CCC(CO)(COC(=O)C(=C)C)COC(=O)C(=C)C         |
| Trimethylolpropane trimethacrylate     |  TRIM                  |&#x2611; |&#x2611;  |&#x2611; | CCC(COC(=O)C(=C)C)(COC(=O)C(=C)C)COC(=O)C(=C)C |
| Vinyl Acrylate                         |   VA                   |&#x2611; |&#x2611;  |&#x2611; | C=COC(=O)C=C |
| Vinyl Methacrylate                     |   VMA                  |&#x2611; |&#x2611;  |&#x2611; | CC(=C)C(=O)OC=C |




<!-- | Functional Monomers to Add             | Acronym | Vina | MIPkit - V |    Smiles   |
| ------------------                     | ------- |      |       |  ---------  |
|                              |         |      |       |          |
|                              |         |      |       |          |
|                              |         |      |       |          |
|                              |         |      |       |          |
|                                        |         |      |       |          |
|                                        |         |      |       |          |
|                                        |         |      |       |          | -->