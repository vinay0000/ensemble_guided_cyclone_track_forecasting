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
└───jupyter_notebooks -- ready-to-run jupyter notebooks with inbuilt documentation
│     └─── sim_data -- data produced during simulation
│  
│
└───docs -- literature
│
│
└───data
│     └─── 2018 -- 2018 Hurricanes in Atlantic basin
│             └─── best_track -- best track data from NHC
│             └─── ensemble   -- ensemble data of GEFS model (ATCF)
│     └─── 2019 
│             └─── best_track
│             └─── ensemble
│     └─── docs -- docs containing info on how to interpret the NHC and ATCF data files

```

Following is description of the scripts:

1. egctf_main : *This is the main-module which contains the EGCTF algorithm and its sub-functions. This module is to be executed prior to invoking the EGCTF algorithm. See the `test_one_case` script for an example of how to utilize this module. This file need not be modified unless the user wishes to make some deeper changes in the EGCTF algorithm.*

2. generate_iterative_ensemble_test_data: *This notebook parses the GEFS ensemble data (ATCF format) and the NHC best-track data and stores the parsed data in python `pickle` object format.*

3. test_one_case: *This notebook executes any user-chosen test-case. Algorithm parameters also maybe configured here.*

4. test_obs_freq: *This notebook analyses the behaviour of the EGCTF performance to varying observation frequency and sensor-noise levels.*

5. test_noise_vs_subseglen: *This notebook analyses the behaviour of the EGCTF performance to varying sensor-noise levels and subsegment lengths.*

6. test_using_ens_slope_vs_linear_extrp: *This notebook compares the behaviour of the EGCTF performance with use of the optimal ensemble track based displacement vector versus the displacement vector obtained from the previous estimated TC positions.*

7. test_many_cases: *The notebook tests all the available test-cases and summarizes the results.*


## Quick Start:

Begin by simply executing the `test_one_case` notebook. 

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