---
hide:
  - navigation
---

# Installation

---

### Installing MIPkit
Installation of MIPkit is easy, but requires a few things to be installed first.

* [Amber and Ambertools](https://ambermd.org/AmberTools.php)
* [GNINA](https://github.com/gnina/gnina) OR [Autodock Vina](https://vina.scripps.edu/downloads/)
* [GROMACS 2024.6](https://manual.gromacs.org/current/install-guide/index.html)
* [Obabel](https://open-babel.readthedocs.io/en/latest/Command-line_tools/babel.html)

It is also highly recommended that CUDA or ROCM is also installed, and GROMACS compiled support for GPU acceleration.

* [CUDA 12.8](https://developer.nvidia.com/cuda-12-8-0-download-archive)
* [ROCM](https://www.amd.com/en/products/software/rocm.html)

To install MIPkit, first create a virtual environment with `python -m venv MIPvenv`. For future use, create a virtual environment activation bash script with :

    source ~/path/to/MIPvenv/bin/activate
    # Through amber
    source ~/path/to/AmberTools24/amber24/amber.sh
    # Or
    source ~/path/to/pmemd24/amber.sh
    source ~/path/to/ambertools25/amber.sh

This will do two things: First, it will start the virtual environment. Second, it will add the ambertools libraries to the PATH so that we can use them with Acpype. 

Finally,

    git clone https://github.com/tj-barrett/BMBT-MIPkit/
    cd BMBT-MIPkit
    pip install BMBT-MIPkit/.

Once installed, `MIPkit -init` to generate sdfs for docking. This will only need to be run again if the FM list is updated.

**Note :** If Vina, GROMACS, and AMBER are not in their default locations, it might be necessary to change the `MIPkit/config/config.yaml` locations to reflect the correct bin locations.

---

### Potential Installation Errors
> * acpype : You might need to install libhdf4-dev, libhdf5-dev first. On Ubuntu 20.04 we experienced an issue with this. Using apt install for both dev packages, then recompiling and installing the Ambertools binary solved the problem.
* acpype : If acpype fails, there might be an issue with the atom typing. Constants.py contains a list of specific-generic conversions, and that list might need to be updated if there is an atom type specified in the pdb that is not recognized by acpype.
* GNINA  : Installation on Ubuntu is much more straightforward than on RHEL (Centos)
* GROMACS : MIPkit was built using 2024.6, so it is recommended. Newer versions should work as well.
