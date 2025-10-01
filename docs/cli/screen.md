---
hide:
  - toc
---
# -screen

`MIPkit -screen ...`

---

**-dockmethod :** `string, default gnina` <br> Specifies whether to use Vina or gnina for docking.

**-fms :** `string, default None` <br> Which functional monomers to screen. If left blank, all FMs will be screened.

**-gmxprotein :** `string, default None` <br> Gromacs processed PDB file used as a docking target in Vina and GROMACS.

**-ncpu :** `int, default #` <br> Number of physical CPU cores to use in both Vina and GROMACS. -1 will use all detected CPUs. Default is a quarter of the physical CPUs detected, rounded down to the nearest 2^n (GROMACS and LAMMPS do weird things with odd CPU counts).

**-protein :** `string, default None` <br> PDB file used as a docking target in Vina and GROMACS. For PDB proteins, -protein should be used instead of -template. If already processed with pdb2gmx, use -gmxprotein instead.

**-template :** `string, default None` <br> PDB file used as a docking target in Vina and GROMACS. -template should be used for non-protein targets, as it avoids the use of pdb2gmx in GROMACS which will throw an error.
