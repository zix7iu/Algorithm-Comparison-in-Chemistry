## General descriptions
[dataset-analysis](./dataset-analysis) contains analysis functions for all datasets

[Algorithm_Accuracy](./dataset-analysis/Algorithm_Accuracy.ipynb) contains the code for all the output in the study

[dataset](./datase) contains the reaction dataset used in this study. 

[dataset_logs](./dataset_logs) contains all the history and logs of generated data used in the study. 

## Installation requirements
The software is written with minimal dependencies in mind. Only the essential packages are required. 
Here is a list of all the packages that need to be installed to run everything.

- python (3.9.16)
- rdkit (2022.9.3)
- pandas (1.5.1)
- numpy (1.23.4)
- scikit-learn (1.1.3)
- scipy (1.9.3)
- pyyaml (6.0)
- matplotlib (3.7.1)
- tqdm (4.64.1)
- gif (22.11.0)

Version numbers are listed just for reference. 
Installing the exact same version is probably not necessary, 
except for things like `matplotlib` that has changed quite a lot from version to version.

Some of the packages are non-essential, for example, `gif` is only needed if you want to make gifs in `chem_analyze.py`;
if you don't need progress bar, you don't need `tqdm` either. Simply create a conda environment, and all of these packages
can be installed via pip or conda.

### For a step-by-step instruction
1. Download a package management system, such as [conda](https://docs.conda.io/en/latest/).
2. In terminal (or other command line applications), create a conda environment named "bandit" for using this software, specify Python version 3.9 (the version we used during development, probably not necessary):

`conda create --name bandit python=3.9`

3. Activate the conda environment:

`conda activate bandit`

4. Install all external packages deebo requires (`Gif` and `rdkit` are only available from pypi):

*Like discussed above, some of the packages are also not essential. For essential packages required, check the import statements for the scripts containing desired functions or classes that will be used.*

`conda install pandas numpy scikit-learn scipy pyyaml matplotlib tqdm`

`pip install rdkit gif`

5. Download the source code folder from GitHub (by clicking "Download").

6. Navigate into the source code folder.

7. All functions and classes can be called, for example, via a Jupyter notebook.


## Author
- Zixuan Liu
