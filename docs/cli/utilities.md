---
hide:
  - toc
---

# utilities

---

These commands are useful utilities that aren't necessary used in the main polymerization and interactions scripts.

**-ABN :** `none` <br> Prints out acidic/basic/neutral breakdown of amino acids for reference.

**-print_feats :** `none` <br> Prints out a list of all FMs with their costs in (eur/mMol) and (eur/Mol).

**-print_feats :** `none` <br> Writes out a csv and images of RDkit pharmacophore features for all FMs and amino acids.

**-print_fms :** `none` <br> Prints out a list of all FMs and their encoded names.

**-print_smiles :** `none` <br> Prints out a list of all FMs and their smiles codes.

**-regen :** `string string, default None None` <br> Regenerates forcefields from PDB files and combined template and complex if both are specified.

**-write_pdb :** `string, default None` <br> Writes out a pdb from the FM list. This is useful if you need to create inputs that adhere to MIPkit molecule orders.

---

These commands are global, but not particularly important unless you need them for any specific reason.

**-basedir :** `string, default None` <br> Creates and uses this directory as the base directory. This probably should be done in bash instead.

**-noclean :** `none, default False` <br> Prevents cleaning. This helps with trouble shooting.

**-timer :** `none, default False` <br> Times the run.

**-verbose :** `none, default False` <br> Makes the runs verbose. Theres a lot of console prints, so probably keep this one off.
