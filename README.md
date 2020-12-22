# Survos_Benchmarking


SuRVoS can be obtained from https://github.com/DiamondLightSource/SuRVoS. For the purpose of Benchmarking we have modifed to add calls to time.time() to measure the exectution time for the Image filters and supervoxel calulations.

The time in seconds is printed to the standard output after the message "Stoped Timing:". Example outputs can be found in the directory for both the Image filters (filter_output.txt) and supervoxel calculations (Supervoxel_output.txt).

To setup Benchmarks simply replace the following files in your SuRvos instalation with the coresponding python files in this repository.

    survos/actions/supervoxels.py

    survos/actions/channels.py

Then rebuild survos as per the instaltion instructions https://diamondlightsource.github.io/SuRVoS/docs/installation/.

To run the benchmark you need to use the GUI to set the 7 filtters shown in the screenshot applied_filters.png using feature channel (on the left hand side of the interfce). You also need to check the settings for the Supervoxel calulations match those given in SuperVoxel_settings.png. All other settings should be left at there default values.

Then you can apply the filters to slice 50 in the test dataset "data.h5" which can be found: https://swanseauniversity-my.sharepoint.com/:f:/g/personal/b_j_thorpe_swansea_ac_uk/EvOJ23JwY91BqWFNN-dOwHkB0dJZxielxcu4ybQagdZZbQ?e=qtQ5ZGwith. 
