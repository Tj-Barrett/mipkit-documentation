---
hide:
  - navigation

---

# Polymerization

---

MIPkit supports two methods of polymerization, implicit and explicit. 

* ***Implicit*** functions off of a single C-C distance cutoff, typically between 3 and 4 Angstrom. 
* ***Explicit*** requires two passes, one from the C-C distance and a second from either carbon and the free-radical forming atoms of the initiator.

### Implicit Polymerization

    MIPkit -react -template CD20_epitope.pdb -mip CD20_MIP_input.pdb -cycles 100 -implicit 0.7 -cutoff 3.3 
       
This will polymerize the CD20_MIP_input structure over 100 cycles (each 2ns long). Every time an eligible C-C pair finds itself below the 3.3 A cutoff, it will have a 70% chance of undergoing a reaction.

### Explicit Polymerization

    MIPkit -react -template CD20_epitope.pdb -mip CD20_MIP_input.pdb -cycles 100 -explicit APS 25 TEMED 1 -cutoff 3.3 5.0
  
This will also polymerize the CD20_MIP_input structure over 100 cycles (each 2ns long). Every time an eligible C-C pair finds itself below the 3.3 A cutoff, it will also need to be within 5.0 A of either the O<sup>-</sup> or O<sup>*</sup> atoms of the decomposed APS. When specifying initiator, the molar ratio should be entered. The proper decomposed number will be calculated automatically (i.e. 25 full APS molecules will decompose into 50 O=S(=O)([O-])[O] ).