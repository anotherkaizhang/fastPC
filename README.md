# fastPC: A Cuda-based Parallel PC Algorithm

The A Cuda-based Parallel PC Algorithm (fastPC) is implemented in PyTorch. Given a dataframe as input, fastPC discovers **causal relationships** between these random variables and outputs a causal graph. It can also perform multiple imputation. 

Corresponding Paper:

## Functionality

* Discovers causal relationships between random variables
* Plots causal graph

Check out the Jupyter Notebook `fastPC Demo` to see a demonstration of the functionality. 
## Prerequisites

### General
* Python >= 3.5
* [PyTorch](https://pytorch.org/get-started/locally/) (tested with PyTorch 1.7.1)
* Optional: CUDA (tested with CUDA 11.0) 

### Required Python Packages:
* numpy
* pandas
* copy
* scipy
* os
* sys
* matplotlib
* pylab
* networkx
* argparse
* [miceforest](https://pypi.org/project/miceforest/)
* itertools
* logging
* torch
* sklearn
* time
* random
* re

### Data
Required: Dataset containing multiple random variables

File format: 
Excel file with header and a column for each random variable. 

#### Data provided
The folder 'data' contains one small dataset for demonstration purposes.

### Running

Check out the Jupyter Notebook `fastPC Demo` to see a demonstration of the functionality. 

Run `fastPC.py --data yourdataset.csv` to run fastPC on your own dataset(s). fastPC will discover causal relationships between random variables in the dataset. 

The causal graph will be plotted as well as saved in the file `graph_excel.xlsx`
_Feel free to improve fastPC use [Issues](https://github.com/kzhang14/fastPC/issues)._  
 
## Paper

Corresponding Paper (peer-reviewed, open access):  
Please cite this paper when using fastPC:
