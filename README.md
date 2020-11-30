# This repository is being updated and shall be available in a useful form after 10th Dec 2020.

# ensemble_guided_cyclone_track_forecasting

This repository contains the python implementation (Jupyter Notebooks) of the EGCTF algorithm as described in the following paper:
V. Ravindra, S. Nag and A. Li, "Ensemble-Guided Tropical Cyclone Track Forecasting for Optimal Satellite Remote Sensing," in IEEE Transactions on Geoscience and Remote Sensing, doi: 10.1109/TGRS.2020.3010821.

The paper can also be found in the folder labelled 'docs'.

## Folder structure:

```
.
│   README.md
│   LICENSE   
│
└───jupyter_notebooks
│   
│   
└───python
│  
│
└───docs
│
│
└───data

```

The scripts under the `python` folder are simply the non-notebook versions of the corresponding jupyter-notebooks contained in the folder `jupyter_notebooks`.
Following is description of the scripts:

1. generate_iterative_ensemble_test_data

2. egctf_main



## Quick Start:

The following line in the script files may need to be revised appropriately (point to the right location) to make the Basemap module work correctly. 
`os.environ["PROJ_LIB"] = "C:\\ProgramData\\Anaconda3\\Library\\share";`

The line was added due to an issue in importing `basemap` (See: https://github.com/conda-forge/basemap-feedstock/issues/30#issuecomment-423512069).


## Funding:
This work has been funded by grants from the National Aeronautics and Space Administration (NASA) Earth Science Technology Office (ESTO) through the Advanced Information Systems Technology (AIST) Program.

## License

Licensed under the MIT License

A short and simple permissive license with conditions only requiring preservation of copyright and license notices. Licensed works, modifications, and larger works may be distributed under different terms and without source code. Please see the LICENSE file in the repository.


## Contact
Feel free to contact me if you have any question:

Vinay Ravindra (vinay.ravindra [at] nasa.gov)
Bay Area Environment Research Institute
NASA Ames Research Center
Moffett Field, CA 94035, USA