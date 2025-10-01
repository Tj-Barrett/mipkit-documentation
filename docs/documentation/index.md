---
hide:
  - toc
---

# Python Module Documentation

---

MIPkit contains many useful scripts for Gromacs and general file i/o that can be used outside of MIPkit by importing the library, including read/write functions for PDBs, itps, atom conversions, etc. 

This section is organized by module, so for example `print_molecule` under `utils` would be imported by `from MIPkit.utils import print_molecule`.


---
## Some important notes

* MIPkit has some quirks, like the need for specific pdb atom orders. When you are creating input files, functional monomers need to adhere to the order RDkit provides from SMILES. If you need to create files seperately, like in the case of hydrogels, use `MIPkit -write_pdb MAA` to write out the necessary methacrylic acid pdb. 

* `/logs` is where all logs are printed during polymerization. If there are any issues during the run, they are likely found in here.