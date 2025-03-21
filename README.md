# multitemporal-s1-backscattering

- This repository is associated to the following article preprint: [https://doi.org/10.5194/egusphere-2025-974](https://doi.org/10.5194/egusphere-2025-974). 

  - This code enables the execution of the SMRT simulations and the reproduction of Figure 9 of the paper, where the simulations results are presented. The model setup is described in detail in Section 3.2 of the paper. The simulations are based on the high-resolution field measurements available on EnviDat [https://doi.org/10.16904/envidat.574](https://doi.org/10.16904/envidat.574), which the user has to provide. Additionally, the chosen snowpack layering and the recorded S1 backscattering for the reference cell are provided in the *./data* folder.

- The other plots presented in the paper are derived from input variations using the same simulation setup of Figure 9.

## Requirements
- The required Python libraries to run the notebook are listed in *./requirements.txt*.

## How to use the notebook
- In a terminal, run the following sequence:
1. `conda create --name <venv> --file ./requirements.txt`
2. `conda activate <venv>`
3. `python -m ipykernel install --user --name=<venv> --display-name "Python (<venv>)"`
- Then, launch:
4. `jupyter notebook`
- Navigate to the project folder, open the notebook, select the kernel associated to the virtual environment just created;
- Run every section of the notebook to reproduce Figure 9 of the paper.

