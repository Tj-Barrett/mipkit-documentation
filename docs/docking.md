---
hide:
  - navigation
---

# Screening and Docking

---

## Recipe Generation

The first step of recipe generation is the identification and analysis of the target epitope. Typically, these targets should prioritize two elements: (i) structure stability and (ii) solvent exposure.

**Stability** is necessary in order to have a consistent target for the MIP cavity to form. 

**Exposure** allows the functional monomers to dock and polymerize about the epitope to actually form the cavity. 

### Screening

    # Screen using just GNINA/VINA
    MIPkit -screen -template CD20-epitope.pdb

    MIPkit -screen -template CD20-epitope.pdb -fms AAM NIPAM BIS AMPSA

    # Screen using GNINA/VINA and GROMACS
    MIPkit -gmxscreen -template CD20-epitope.pdb

    MIPkit -gmxscreen -template CD20-epitope.pdb -fms AAM NIPAM BIS AMPSA

Following the selection of the epitope, all functional monomers present in `./constants/fm_list.yaml` can be screened against the template using Autodock Vina or GNINA. Alternatively, `-fms` can be used to specify which functional monomers should be screened. [Supported Functional Monomers](./fms.md) contains a list of supported functional monomers for MIPkit, GNINA, and Vina. Docking method can be changed using `-dockmethod`.

`-gmxscreen` adds an additional interaction run to the docked FM and results in single FM H-bonds, energies, and RDF. This provides more insight into the template-FM interactions of the system, providing a better basis for recipe generation.

### Precomplexation / Recursive Docking

    MIPkit -dock -config CD20_MD.yaml

    MIPkit -dock -template CD20-epitope.pdb -fms AAM 5 NIPAM 14 BIS 3 AMPSA 1

Precomplexes are formed by recursively docking functional monomers on the surface of the template. By default, the functional monomers are docked serially. In the above example, that means 5 AAM will be docked, followed by 14 NIPAM, then 3 BIS, and finally 1 AMPSA. More details on the differences this creates can be found in the [CD20 Example](./quickstart/cd20.md). Alternatively, `-shuffle` can be used to randomize the structure. 

`-dock` will determine the box shape based on the overall size of the template to perform blind docking. If you wish to restrict docking to a specific region, use a `-config` file with custom box dimensions. `-dockmethod` can be used to specify `gnina` or `vina` for docking and screening.