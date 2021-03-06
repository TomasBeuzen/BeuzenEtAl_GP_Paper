[![DOI](https://zenodo.org/badge/144752081.svg)](https://zenodo.org/badge/latestdoi/144752081)

This is a repository for the paper:

## Ensemble models from machine learning: an example of wave runup and coastal dune erosion
### Tomas Beuzen<sup>1</sup>, Evan B. Goldstein<sup>2</sup>, Kristen D. Splinter<sup>1</sup>

<sup>1</sup>Water Research Laboratory, School of Civil and Environmental Engineering, UNSW Sydney, NSW, Australia

<sup>2</sup>Department of Geography, Environment, and Sustainability, University of North Carolina at Greensboro, Greensboro, NC, USA
 
**Citation:** Beuzen, T, Goldstein, E.B., Splinter, K.S. (In Review). Ensemble models from machine learning: an example of wave runup and coastal dune erosion,
Natural Hazards and Earth Systems Science, SI Advances in computational modeling of geoprocesses and geohazards.

<img src="docs/figure.png" 
     width="800"
     class="center" />

The folder `paper_code` contains a jupyter notebook that reproduces the GP runup predictor presented in the manuscript.

The folder `LEH04model` contains Python scripts for using the GP runup predictions from the 2011 storm in the Larson, Erikson, Hanson (2004) dune erosion model.

The folder `data_repo` contains data required to run the code.
* The file `lidar_runup_data_for_GP_training.csv` contains the 416 runup samples used to develop the GP predictor.
* The file `lidar_runup_data_for_GP_testing.csv` contains 50 additional runup samples for the purpose of testing the GP predictor.
* Additional data including runup observations and dune erosion observations used with the manuscript are not yet publicly available. Please email the lead author for details.

For first-time users, it is recommended to install the Anaconda Distribution from:
https://www.anaconda.com/distribution/.

The packages required to run the Jupyter notebooks are included in `requirements_win64.txt`. To install, do the following:
* Open a Windows Command Processor 
* Create a new environment using: `conda create -n "envGP" --file requirements_win64.txt`
* Activate that environment using: `conda activate envGP`
* Change to the directory where the notebook is located, e.g: `cd C:\Users\TomasBeuzen\BeuzenEtAl_2019_NHESS_GP_runup_model\paper_code`
* Run jupyter notebooks using: `jupyter notebook`

Jupyter notebooks will open in a new html window. Simply select the notebook to open it. To run notebook cells, use `shift + enter`.

For more information on using jupyter notebooks, see the documentation at https://jupyter.org/
