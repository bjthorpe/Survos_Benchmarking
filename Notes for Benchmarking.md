SuRVoS can be obtained from https://github.com/DiamondLightSource/SuRVoS. For the purpose of Benchmarking we have modifed to add calls to time.time() to measure the exectution time for the Image filters and supervoxel calulations.

The time in seconds is printed to the standard output after the message "Stoped Timing:". Example outputs can be found in the directory for both the Image filters (filter_output.txt) and supervoxel calculations (Supervoxel_output.txt).

To setup Benchmarks simply replace the following files in your SuRvos instalation with the coresponding python files in this directory.

  + survos/actions/supervoxels.py

  + survos/actions/channels.py
  
Then rebuild survos as per the instaltion instructions https://diamondlightsource.github.io/SuRVoS/docs/installation/. 
 
To run the benchmark you need to use the GUI to set the 7 filtters shown in the screenshot applied_filters.png using feature channel (on the left hand side of the interfce). You also need to check the settings for the Supervoxel calulations match those given in SuperVoxel_settings.png. Then you can apply the filters to slice 50 in the test dataset "data.h5" with all other settings were left at there default values.




