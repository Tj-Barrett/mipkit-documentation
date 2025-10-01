---
hide:
  - toc
---
# -gmxscreen

`MIPkit -gmxscreen ...`

---

This command takes a combination of `-screen` and `-interact` arguments. The most relevant ones are listed here.

## -screen arguments

**-dockmethod :** `string, default gnina` <br> Specifies whether to use Vina or gnina for docking.

**-gmxprotein :** `string, default None` <br> Gromacs processed PDB file used as a docking target in Vina and GROMACS.

**-fms :** `string, default None` <br> Which functional monomers to screen. If left blank, all FMs will be screened.

**-ncpu :** `int, default #` <br> Number of physical CPU cores to use in both Vina and GROMACS. -1 will use all detected CPUs. Default is a quarter of the physical CPUs detected, rounded down to the nearest 2^n (GROMACS and LAMMPS do weird things with odd CPU counts).

**-protein :** `string, default None` <br> PDB file used as a docking target in Vina and GROMACS. For PDB proteins, -protein should be used instead of -template. If already processed with pdb2gmx, use -gmxprotein instead.

**-template :** `string, default None` <br> PDB file used as a docking target in Vina and GROMACS. -template should be used for non-protein targets, as it avoids the use of pdb2gmx in GROMACS which will throw an error.

## -interact arguments

**-fs :** `str, default None` <br> Timestep in femtoseconds. Options are 05 (0.5), 1 (1.0), 2 (2.0). 

**-gpu_id :** `int, default None` <br> A direct wrap to the command in GROMACS. Sets the GPU ID number in machines with multiple GPUs.

**-ns :** `int, default None` <br> Nanosecond duration for interaction to occur. Options are 50, 100, 300, and 500. 

**-solvent :** `string, named. default spc` <br> The solvent in the system. Defaults to water, but DMSO is also currently supported. Additional solvents will be added as needed.
