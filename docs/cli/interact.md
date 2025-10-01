---
hide:
  - toc
---

# -interact
`MIPkit -interact ...`

---


**-config :** `string, default None` <br> The recipe file to be used with `-id`.

**-cplx :** `string, default None` <br> The complex, nanogel, or polymer file to be reacted. This file is the one analyzed by the polymerization algorithm.

**-fs :** `str, default None` <br> Timestep in femtoseconds. Options are 05 (0.5), 1 (1.0), 2 (2.0). 

**-gmxprotein :** `string, default None` <br> Gromacs processed PDB file used as a docking target in Vina and GROMACS.

**-gpu_id :** `int, default None` <br> A direct wrap to the command in GROMACS. Sets the GPU ID number in machines with multiple GPUs.

**-id :** `none, default False` <br> Must be used with `-config` to get the initial FM recipe. `-id` decomposes any polymer chains into their constituent components to get pairwise FM-Template interactions in the system. 

**-ncpu :** `int, default #` <br> Number of physical CPU cores to use in both Vina and GROMACS. -1 will use all detected CPUs. Default is a quarter of the physical CPUs detected, rounded down to the nearest 2^n (GROMACS and LAMMPS do weird things with odd CPU counts).

**-offset :** `float float float, default 0 0 0` <br> Offsets template molecule from center by x, y, z. This is necessary for NIP interactions, where the final state of the template molecule does not exist.

**-posre :** `int, default 1000` <br> A direct wrap to the command in GROMACS. Sets the position restraints of the template or protein target. 

**-protein :** `string, default None` <br> PDB file used as a docking target in Vina and GROMACS. For PDB proteins, -protein should be used instead of -template. If already processed with pdb2gmx, use -gmxprotein instead.

**-regen :** `none, default False` <br> Regenerates the AMBER forcefields using Acpype. This is likely unnecesary, but might be helpful when you have a final state but not the forcefield parameters.

**-solvent :** `string, named. default spc` <br> The solvent in the system. Defaults to water, but DMSO is also currently supported. Additional solvents will be added as needed.

**-template :** `string, default None` <br> PDB file used as a docking target in Vina and GROMACS. -template should be used for non-protein targets, as it avoids the use of pdb2gmx in GROMACS which will throw an error.

**-wash :** `none, default False` <br> Removes all unreacted monomers from the system, simulating a hot or cold wash during MIP development. In reality, polymerized complexes WITH excess functional monomers are not MIPs at all, and are therefore unrealistic representations. This allows us to measure the interaction energies of full complexes to compare against unpolymerized systems, and to compare full complexes to MIPs. 
