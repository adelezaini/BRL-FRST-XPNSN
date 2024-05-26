
## General
General functions processing Xarray Dataset/DataArray

- `coordinate_operations.py`: different operations related to the spatial dimensions of DataArrays, such as conversion of longitudes unit system, land surface model coordinates, landunit-related values, filter DataArray with a given list of lon-lat coordinates ...
- `regrid.py`: regrid a Dataset with xesmf Regrider
- `fit.py`: fit with a polynomial or a gaussian curves

## Preprocessing:
Functions of import, convert PFTs and apply the vegetation perturbations to the original surfdata_map input file

- `read-lpjguess-files`: import data as DataArray from LPJ-GUESS output files
- `convert-pfts.py`: convert PFTs from LPJ-GUESS to CLM5
- `preprocess.py`: perform preprocessing on surfdata_map file, mostly related to performing the idealized configuration change and applying the vegetation perturbations to the original input file

## Postprocessing:
- `postprocess.py`: skim and fix the ouputs, such as units, variables... while applying operations to evaluate new ones (eg. Ghan's decomposition). The postprocessed data is saved in netCDF files named e.g. IDEAL-ON_BVOC_20082012.nc

## Plotting:
- `plot.py`: plots for Figures
- `plot-pfts.py`: produce extra plots in support of exploring the datasets and of the analysis process
- `palette.py`: create costumed colour palettes for plots

side note: fix 'scomposition', names as titles
