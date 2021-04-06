# Sentinel-2-GEE

## General information
This repository fetches Sentinel-2 data from Google Earth Engine.

The script 02 downloads data of one scene. The script 04 downloads data of multiple scenes of multiple time periods. As there is a limitation on the amount of data can be downloaded at a time, script 04 downloads data band by band, and script 05 assembles these bands to an unified data file.

The scripts apply a cloud remove solution that is implemented in "sentinel_2_cloud_free.py". It was introduced in [1]. Related repositories and paper are listed below

https://github.com/SiPEO/GEE_DataDownloader

https://github.com/SiPEO/GEE_Utils.

Schmitt, Michael, et al. "Aggregating cloud-free Sentinel-2 images with Google earth engine." PIA19: Photogrammetric Image Analysis (2019): 145-152.

## Environment
The scripts is operated in a conda environment with jupyter notebook.

The "my_gee_env.yml" file provides the identical conda environment under which the scripts operate. To generate a conda env with yml file, please see the following link: https://conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html#creating-an-environment-from-an-environment-yml-file

## Additional information
As an example, the file "toulouse.geojson" gives the geographic extent of a region-of-interest ROI. 

Great learning resource can be find here: https://github.com/giswqs/geemap
