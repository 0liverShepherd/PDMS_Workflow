# PDMS Workflow

This repository contains the workflow used to build, simulate, and analyse PDMS systems using OpenFF, LAMMPS, and bespoke force field parameters.

## Installation

Create the environment from the provided YAML file:

```bash
mamba env create -f environment.yaml
conda activate Polymer
```

## Content

- Notebook ***`pdms_lammps_workflow.ipynb`*** Contains the full workflow and analysis for the project. 
- Custom OpenFF force field used throughout the workflow ***`bespoke_ff.offxml`***. Created using OpenFF Sage v2.3.0, with aditional silicon parameters adopted from OPLS-AA as show in Table S4 of: 
"https://pubs.acs.org/doi/10.1021/acs.jpcb.4c08471?fig=fig3&ref=pdf" 

The resulting force fiels was processed using the Presto workflow: 
"https://github.com/cole-group/presto/blob/main/"

- ***`environment.yaml`*** Conda environment specification file for reproducing the software environment used in this work.
- ***`README.md`*** Repository documentation and usage instructions
