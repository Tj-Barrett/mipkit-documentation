---
hide:
  - toc
---
# -cost


`MIPkit -cost ...`

---

**-config :** `string, default None` <br> Uses config recipe to generate cost estimate.

**-fms :** `string int ... , default None` <br> Takes the place of -config in specifying the functional monomer names and count for the recipe. For example, `-cost -fms NIPAM 15 AAC 10 BIS 2` will use a recipe containing 15 NIPAM, 10 AAC, and 2 BIS, and estimates the cost in eur/mMol as € 6.45.