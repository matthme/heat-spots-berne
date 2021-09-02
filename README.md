[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/matthme/heat-spots-berne/HEAD?filepath=Heatmap.ipynb)

# Wärmcity Bern

We are trying to reproduce and interpret research of climate scientists into mapping and modelling of heat spots, or urban heat islands in the city using DIY (low cost and accessible-build) temperature sensors.

This is a project started at the [#EnergyClimateHack](https://hack.opendata.ch/project/762) hackathon on August 31, 2021. For more background visit the [challenge page here](https://hack.opendata.ch/project/674), and contact us via GitHub issues or the Slack channel if you have questions.

See also [NOTES.md](NOTES.md) for a sketch of our app idea, additional links and references.

## Data

This repository contains data collected during three heat waves in Berne, Switzerland, during June 2018, June 2019, and July 2019.

The dataset was created and published by the [Climatology Group of the Institute of Geography](https://www.geography.unibe.ch/research/climatology_group/research_projects/urban_climate_bern/index_eng.html) (Oeschger Centre for Climate Change Research, University of Bern), available as open access at [Burger, Gubler, Heinimann, Brönnimann 2021](https://www.sciencedirect.com/science/article/pii/S2212095521001152?via%3Dihub#s0160).

We made an effort to "harmonize" the timestamp fields in the data, i.e. put them all in the same UTC format (some of them were only with AM/PM or vorm./nachm. indication). Both the original (`1-s2*.csv`) and adjusted (`data_harmonized*.csv`) data is in the `data` subfolder, along with the locations of the sensors (`Metadata_Logger`).

This is complemented by meteorological variables (Radiation, Precipitation, Wind speed, Wind direction & Temperature) from the official measurement station in Zollikofen during the same three heatwaves. See `Met_Zoll*.csv`. *Caution!* During hw18 wind speed was measured in m/s, during hw191 and hw192 it was measured in km/h.

We have ensured all data is in UTF-8 and a Simple Data Format (CSV), and created a [Data Package](datapackage.json) containing all the readings and control measures. This can be validated and explored with [Frictionless Data](https://frictionlessdata.io) tools.

## Explore

This repository includes a [Jupyter](https://jupyter.org) data science notebook which you can [preview here](https://nbviewer.jupyter.org/github/matthme/heat-spots-berne/blob/main/Heatmap.ipynb) (nbviewer) to facilitate the sharing and further analysis and development using the latest open data sharing standards.

To start a cloud-hosted notebook that you can run and modify, use [Binder](https://mybinder.org/v2/gh/matthme/heat-spots-berne/HEAD?filepath=Heatmap.ipynb) or [Colab](https://colab.research.google.com/github/matthme/heat-spots-berne/blob/main/Heatmap.ipynb).

## Slightly slower start

To get this running on your local machine, we suggest:

1. Install [Anaconda](https://anaconda.org/) and open a shell in the root folder of this project.
2. Create a new environment using `conda env create -n heatspots -f=environment.yml`
3. Run the command `jupyter notebook` to start Jupyter

You will see an initial Heatmap visualization. Click "Run all".

# License

This project is open source using the [MIT License](LICENSE)
