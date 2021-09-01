[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/matthme/heat-spots-berne/HEAD?filepath=Heatmap.ipynb)

# The heat spots of Berne

Here we are trying to reproduce and interpret research of climate scientists into mapping and modelling of urban heat islands in the city using DIY (low cost and accessible-build) temperature sensors.

This repository contains data collected during three heat waves in Berne, Switzerland, during June 2018, June 2019, and July 2019. The dataset was created and published by the [Climatology Group of the Institute of Geography](https://www.geography.unibe.ch/research/climatology_group/research_projects/urban_climate_bern/index_eng.html) (Oeschger Centre for Climate Change Research, University of Bern), available as open access at [Burger, Gubler, Heinimann, Brönnimann 2021](https://www.sciencedirect.com/science/article/pii/S2212095521001152?via%3Dihub#s0160). 

We have created a [Data Package](https://frictionlessdata.io) with a harmonized version of the sensor readings, as well as their locations and official meteorological indicators for reference. There is also a [Jupyter Notebook](https://jupyter.org) to facilitate the sharing and further analysis and development using the latest open data sharing standards.

This is a project started at the [#EnergyClimateHack](https://hack.opendata.ch/project/762) hackathon on August 31, 2021. For more background visit the [challenge page here](https://hack.opendata.ch/project/674), and contact us via GitHub issues or the Slack channel if you have questions.

## Quickstart

Click here to start a cloud-hosted notebook that you can edit and run:

[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/matthme/heat-spots-berne/HEAD?filepath=Heatmap.ipynb)

## Slightly slower start

To get this running on your local machine, we suggest:

1. Install [Anaconda](https://anaconda.org/) and open a shell in the root folder of this project.
2. Create a new environment using `conda env create -n heatspots -f=environment.yml`
3. Run the command `jupyter notebook` to start Jupyter

You will see an initial Heatmap visualization. Click "Run all".

# License

This project is open source using the [MIT License](LICENSE)