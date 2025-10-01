---
hide:
  - toc
---
# -dock


`MIPkit -dock ...`

---

**-config :** `string, default None` <br> The recomended docking approach. Specifies all or some inputs in the config rather than via command line.

**-dockmethod :** `string, default gnina` <br> Specifies whether to use Vina or gnina for docking.

**-fms :** `string int ... , default None` <br> Takes the place of -config in specifying the functional monomer names and count to be docked. For example, `-dock -fms NIPAM 15 AAC 10 BIS 2` will dock 15 NIPAM, 10 AAC, and 2 BIS.

**-gmxprotein :** `string, default None` <br> Gromacs processed PDB file used as a docking target in Vina and GROMACS.

**-ncpu :** `int, default #` <br> Number of physical CPU cores to use in both Vina and GROMACS. -1 will use all detected CPUs. Default is a quarter of the physical CPUs detected, rounded down to the nearest 2^n (GROMACS and LAMMPS do weird things with odd CPU counts).

**-protein :** `string, default None` <br> PDB file used as a docking target in Vina and GROMACS. For PDB proteins, -protein should be used instead of -template. If already processed with pdb2gmx, use -gmxprotein instead.

**-scale :** `int, default 1` <br> This command scales the FM recipe by multiplying the number of functional monomers by the scaled amount. This allows for increasing systems in order to determine saturation.

**-serial :** `none, default False` <br> If -serial is flagged, the functional monomers will be docked in the order in which they are specified. For example, 15 NIPAM, 10 AAC, and 2 BIS will dock all 15 NIPAM, then 10 AAC, then the 2 BIS. This can be used to determine whether docking functional monomers before crosslinkers is important to performance or not.

**-shuffle :** `none, default True` <br> Shuffles the input FM. So, for 5 NIPAM, 1 AAC, and 2 BIS, we might see a docked order of \[ NIPAM, BIS, BIS, AAC, NIPAM, NIPAM, NIPAM, NIPAM \].

**-shuffle_seed :** `string, default xF00D` <br> Controls the shuffle order. This is necessary for validation.

**-template :** `string, default None` <br> PDB file used as a docking target in Vina and GROMACS. -template should be used for non-protein targets, as it avoids the use of pdb2gmx in GROMACS which will throw an error.
