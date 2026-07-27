# PDMS Workflow

## Workflow

1. Build PDMS chains
2. Initialise box coordinates
3. Assign force field parameters
4. Generate LAMMPS inputs
5. Energy minimisation
6. Equilibration
7. Production MD
8. Post-processing and analysis

## Installation

Clone Repository:

```bash
git clone https://github.com/0liverShepherd/PDMS_Workflow.git
```

Create environment from the provided YAML file:

```bash
mamba env create -f environment.yaml
conda activate Polymer
```

## Content

- ***`pdms_lammps_workflow.ipynb`*** Contains the full workflow and analysis for the project. 
- ***`bespoke_ff.offxml`*** Custom OpenFF force field used throughout the workflow. Created using OpenFF Sage v2.3.0, with aditional silicon parameters adopted from OPLS-AA as show in Table S4 of: 
"https://pubs.acs.org/doi/10.1021/acs.jpcb.4c08471?fig=fig3&ref=pdf" 
The resulting bespoke force field was produced using the Presto workflow: 
"https://github.com/cole-group/presto/blob/main/"
- ***`environment.yaml`*** Conda environment specification file for reproducing the environment used in this work.
- ***`README.md`*** Repository documentation and usage instructions
