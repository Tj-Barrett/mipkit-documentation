---
hide:
  - toc
---
# -react

`MIPkit -react ...`

---

**-box :** `int int int, default 10 10 10` <br> A direct wrap to the command in GROMACS. Controls the size of the solvent box the MIPs are created in.

**-cplx :** `string, default None` <br> The complex, nanogel, or polymer file to be reacted. This file is the one analyzed by the polymerization algorithm.

**-cutoff :** `float (float), default 3.0 (5.0)` <br> Takes up to two arguments, with the second reserved only for -explicit simulations. The first cutoff value represents the distance cutoff between eligible reacting atoms. The second cutoff represents the distance cutoff between APS intiators and eligible reacting atoms.

**-cycles :** `int, default 10` <br> The total number of polymerization cycles to run.

**-explicit :** `string int ..., default APS 10 TEMED 1` <br> Makes the polymerization method [explicit](../polymerization.md). -explicit takes string int pairs as arguments. The string specifies the molecule and the int the molar ratio. [Polymerization](../polymerization.md) goes into more detail on the selection of these molar ratios.

**-gmxprotein :** `string, default None` <br> Gromacs processed PDB file used as a docking target in Vina and GROMACS.

**-gmxt :** `string, named. default "default"` <br> Assigns which time will be used per cycle. Options are `short` for 0.5 ns, `default` 2.0 for ns, and `long` for 5.0 ns.  

**-gpu_id :** `int, default None` <br> A direct wrap to the command in GROMACS. Sets the GPU ID number in machines with multiple GPUs.

**-implicit :** `float, default 1` <br> Makes the polymerization method [implicit](../polymerization.md). In short, implicit assumes that reaction is possible 

**-parallel :** `string, default None` <br> Modifies the RXN and RES folders created by Acpype, as well as the work, comp, and log directories. Realistically, different runs should be run in different directories but this allows you to run multiple in the same place if you desire.

**-min :** `none, default False` <br> Takes no argument, and simply flags whether a 10 ns starting equilibration / minimization from the docked configuration should occur before the polymerization cycles begin. Default `False`.

**-ncpu :** `int, default #`<br> Number of physical CPU cores to use in both Vina and GROMACS. -1 will use all detected CPUs. Default is a quarter of the physical CPUs detected, rounded down to the nearest 2^n (GROMACS and LAMMPS do weird things with odd CPU counts).

**-posre :** `int, default 1000` <br> A direct wrap to the command in GROMACS. Sets the position restraints of the template or protein target. 

**-protein :** `string, default None` <br> PDB file used as a docking target in Vina and GROMACS. For PDB proteins, -protein should be used instead of -template. If already processed with pdb2gmx, use -gmxprotein instead.

**-restart :** `none, default False` <br> Restart from a previous step. Needs to be the specific `step*...` complexes and templates.

**-solvent :** `string, named. default spc` <br> The solvent in the system. Defaults to water, but DMSO, DMF, CHL, and MeCN are supported.

**-shell :** `string, default None`<br> Shell script used to replace the standard cycles. There are various lengths built in (.5 ns, 2 ns, 5 ns), however if you would like to use a custom method that does not fit through the modification of existing files, use this. Input and Output must adhere to the MIPkit nomenclature in order to work properly.

**-template :** `string; default None` <br> PDB file used as a docking target in Vina and GROMACS. -template should be used for non-protein targets, as it avoids the use of pdb2gmx in GROMACS which will throw an error.
