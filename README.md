# p22c-esgf-processing
Post-processing of data that have been downloaded from ESGF, including CMIP6 data.

## Requirements and setup
Data should already have been downloaded from ESGF (e.g. using [p22b-esgf-globus](https://github.com/grandey/p22b-esgf-globus).

Software requirements - including [CDO (Climate Data Operators)](https://code.mpimet.mpg.de/projects/cdo/) - can be installed via the [environment.yml](environment.yml) file with `conda`:
```
conda env create --file environment.yml
conda activate p22c-esgf-processing
```

If [environment.yml](environment.yml) has been modified, then recreate the environment from scratch using the `--force` option:
```
conda env create --file environment.yml --force
```
(Note: `conda env update --prune` does not currently appear to work as expected - see https://github.com/conda/conda/issues/7279.)

## Author
B. S. Grandey (Nanyang Technological University), in collaboration with colleagues at NTU.

## Acknowledgements
This research / project is supported by the National Research Foundation, Singapore, and Ministry of National Development, Singapore under its Urban Solutions and Sustainability Integration Fund (Award No.: USS-IF-2020-3).
