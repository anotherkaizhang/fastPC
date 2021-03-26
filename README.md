# fastPC: A Cuda-based Parallel PC Algorithm

The A Cuda-based Parallel PC Algorithm (fastPC) is implemented in PyTorch. Given a dataframe as input, fastPC discovers **causal relationships** between these random variables and outputs a causal graph. It can also perform multiple imputation. 

Paper:

## Functionality

* Discovers causal relationships between random variables
* Plots causal graph

Check out the Jupyter Notebook `fastPC Demo` to see a demonstration of the functionality. 
## Prerequisites

### General
* Python >= 3.5
* [PyTorch](https://pytorch.org/get-started/locally/) (tested with PyTorch 1.7.1)
* matplotlib>=3.3.3 
* miceforest>=2.0.3 (https://pypi.org/project/miceforest/)
* networkx>=2.5
* numpy>=1.19.2
* pandas>=1.1.3
* scikit-learn>=0.24.1
* Optional: CUDA (tested with CUDA 11.0) 

### Other Required Python Packages:
* os
* sys
* argparse
* itertools
* logging
* time


### Data
Required: Dataset containing multiple random variables

File format: 
Excel file with header and a column for each random variable. 

#### Data provided
The folder 'data' contains one small dataset for demonstration purposes.

### Running

Check out the Jupyter Notebook `fastPC Demo` to see a demonstration of the functionality. 

Run `fastPC.py --data yourdataset.csv` to run fastPC on your own dataset(s). fastPC will discover causal relationships between random variables in the dataset, and outputs a completed partially directed acyclic graph (CPDAG). 

The causal graph will be plotted as well as saved in three files:
`graph_excel.csv`: contains all edges in the CPDAG;
`graph_excel_bidirection.csv`: only the bidirection edges in the CPGAD;
`graph_excel_single_direction.csv`: only the single direction edges in the CPGAD.

_Feel free to improve fastPC use [Issues](https://github.com/kzhang14/fastPC/issues)._  
 
## Paper

Corresponding Paper (peer-reviewed, open access):  
Please cite this paper when using fastPC:
