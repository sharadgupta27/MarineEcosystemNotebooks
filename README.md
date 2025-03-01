# Marine Ecosystem Notebooks

[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/gaelforget/Cbiomes2019Notebooks/master)
[![DOI](https://zenodo.org/badge/185446209.svg)](https://zenodo.org/badge/latestdoi/185446209)

[Jupyter](https://jupyter.org) / [Julia](https://julialang.org) notebooks that use marine ecosystem models and observations. They illustrate:

1. how differential equation solvers can be used to integrate models in time
1. how ocean colour data and [CBIOMES](https://https://github.com/CBIOMES) model ouptut can be used jointly
1. how model output and data available online are easily accessed in `julia`

<p align="center">
  <img width="400" src="https://github.com/gaelforget/MarineEcosystemNotebooks/blob/master/figs/RandomFlow.gif?raw=true">
</p>

## Ocean Color And Biomes

1. `OceanColourAlgorithms.ipynb` provides simple recipes to compare [CBIOMES model output](https://github.com/gaelforget/CBIOMES) and [ocean color data](https://www.oceancolour.org).
1. `ModelReflectanceMap.ipynb` uses `Plots.jl` to map out [CBIOMES model output](https://github.com/gaelforget/CBIOMES) and [ocean color data](https://www.oceancolour.org).
1. `Classifications.ipynb` applies the [OC-CCI](https://www.oceancolour.org) classifier ([Jackson et al 2017](http://doi.org/10.1016/j.rse.2017.03.036)) over a 2D region.
1. `ClassificationTestbed.ipynb` puts together a series of variables aimed at testing various classification algorithms based on [CBIOMES model output](https://github.com/gaelforget/CBIOMES).

## Accessing Data And Model Output

1. `DarwinModelOutput.ipynb` uses either (1) the [MIT-CBIOMES opendap](http://engaging-opendap.mit.edu:8080/las/) server or (2) the [Simons CMAP](https://cmap.readthedocs.io/en/latest/) data base to access model output from the [CBIOMES](https://cbiomes.org) project.
2. `GradientsCruiseData.ipynb` uses [Simons' CMAP](https://cmap.readthedocs.io/en/latest/) to download [SCOPE-Gradients](http://scope.soest.hawaii.edu/data/gradients/data/) and then plots the data in `julia` using the `Plots.jl` package.
3. `ArgoProfileData.ipynb` uses [Argo](https://doi.org/10.3389/fmars.2019.00439), obtained from the IFREMER [GDAC](http://www.argodatamgt.org/Access-to-data/Access-via-FTP-on-GDAC), to look at variability in temperature and salinity through time, taking a North Pacific region as an example.

## Mechanistic And Probabilistic Models

1. `Models/EpiGen_notebook.jl` is a Julia translation of the `EpiGen` model of [Walworth et al 20](www.pnas.org/cgi/doi/10.1073/pnas.1919332117)

## Differential Equations

Here are examples that show how to use the differential equations package.

1. `SolidBodyRotation.ipynb` simulates a single trajectory in an idealized flow field (e.g. solid body rotation)
1. `RandomFlow_fleet.ipynb` simulates a cloud of particles in a randomly generated eddy field (e.g. meso-scale).

## _Notes:_

- _Each `.ipynb` notebook is paired with a `.jl` file via `jupytext`_
- _An interactive version can readily be spun up via the `launch binder` badge_
- _Please use the [repository issue tracker](https://guides.github.com/features/issues/) for queries, bug reports, new contributions, etc._
- _The `src/` folder contains helper functions & scripts._

