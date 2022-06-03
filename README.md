# WSCBS2022
[![DOI](https://zenodo.org/badge/498536259.svg)](https://zenodo.org/badge/latestdoi/498536259)

###
### Development

We use two submodules for the data_processing package and visualization package of this repository. To clone the repository, run:
```bash
git clone --recurse-submodules https://github.com/Han-Linnn/WSCBS2022.git
```

or alternatively, run
```bash
git submodule init
git submodule update
```
###
### Build Brane Package and Pipline

The Python scripts (data_processing.py, visualization.py, test_visualization.py, test_preprocessing.py), the corresponding container.yml files and the train.csv and test.csv are initially required to get started.

First run:

```bash
brane login http://localhost:8080 --username linhan
```

Then run :

```bash
 make build 
``````
To build and push all packages

###
### Running the pipeline
At that point start an ide (make start-ide whereever brane's make file is) and upload your local `Pipeline.ipynb ` file to jupyters and run the cells in `Pipeline.ipynb` in jupyterlab to get started. Then this should take like max a minute and then return the processed data `preprocessing.csv` and the visualization outputs.
