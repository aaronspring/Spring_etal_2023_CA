# Spring et al. 2023

A manuscript to be submitted to Climate Action.

## Aim

This repo is setup for scientists interested to reproduce our `Spring et al., 2023` paper. It contains scripts to reproduce the analysis and create the shown figures. It is inspired by `Irving (2015)` to enhance reproducibility in geosciences.

-   Irving, Damien. “A Minimum Standard for Publishing Computational Results in the Weather and Climate Sciences.” Bulletin of the American Meteorological Society 97, no. 7 (October 7, 2015): 1149–58. <https://doi.org/10/gf4wzh>.

## Climate model setup

- Mauritsen, T., Bader, J., Becker, T., Behrens, J., Bittner, M., Brokopf, R., Brovkin, V., Claussen, M., Crueger, T., Esch, M., Fast, I., Fiedler, S., Fläschner, D., Gayler, V., Giorgetta, M., Goll, D. S., Haak, H., Hagemann, S., Hedemann, C., … Roeckner, E. (2019). Developments in the MPI‐M Earth System Model version 1.2 (MPI‐ESM1.2) and Its Response to Increasing CO 2. Journal of Advances in Modeling Earth Systems, 11(4), 998–1038. doi: 10/gftpps

- Fiedler, S., Wyser, K., Rogelj, J., & van Noije, T. (2020). Radiative effects of reduced aerosol emissions during the COVID-19 pandemic and the future recovery [Preprint]. Climatology (Global Change). doi: 10.1002/essoar.10504704.1

- Forster, P. M., Forster, H. I., Evans, M. J., Gidden, M. J., Jones, C. D., Keller, C. A., Lamboll, R. D., Quéré, C. L., Rogelj, J., Rosen, D., Schleussner, C.-F., Richardson, T. B., Smith, C. J., & Turnock, S. T. (2020). Current and future global climate impacts resulting from COVID-19. Nature Climate Change, 1–7. doi: 10/gg7s7w

- Jones, C. D., Hickman, J. E., Rumbold, S. T., Walton, J., Lamboll, R. D., Skeie, R. B., Fiedler, S., Forster, P. M., Rogelj, J., Abe, M., Botzet, M., Calvin, K., Cassou, C., Cole, J. N. S., Davini, P., Deushi, M., Dix, M., Fyfe, J. C., Gillett, N. P., … Ziehn, T. (2021). The Climate Response to Emissions Reductions Due to COVID-19: Initial Results From CovidMIP. Geophysical Research Letters, 48(8), e2020GL091883. doi: 10/gjpjdj

- Lamboll, R. D., Jones, C. D., Skeie, R. B., Fiedler, S., Samset, B. H., Gillett, N. P., Rogelj, J., & Forster, P. M. (2021). Modifying emissions scenario projections to account for the effects of COVID-19: protocol for CovidMIP. Geoscientific Model Development, 14(6), 3683–3695. doi: 10.5194/gmd-14-3683-2021


## Packages used

-   model output aggregation: `cdo`, `pymistral`
-   analysis: `xarray`
-   visualisation: `matplotlib`, `cartopy`, `seaborn`

## Computation

The results in this paper were obtained using a number of different software packages. The command line tool known as Climate Data Operators (CDO) was used to aggregate output and perform routine calculations on those files (e.g., the calculation of temporal and spatial means). For more complex analysis and visualization, a Python distribution called Anaconda was used. A Python library called `xarray` was used for reading/writing netCDF files and data analysis. `matplotlib` (the default Python plotting library) and `cartopy` were used to generate the maps. The high-dimensional global aggregation plots are done with `seaborn`.

-   CDO: Climate Data Operators, 2018. <http://www.mpimet.mpg.de/cdo>.
-   Hoyer, Stephan, and Joe Hamman. “Xarray: N-D Labeled Arrays and Datasets in Python.” Journal of Open Research Software 5, no. 1 (April 5, 2017). <https://doi.org/10/gdqdmw>.
-   Hunter, J. D. “Matplotlib: A 2D Graphics Environment.” Computing in Science Engineering 9, no. 3 (May 2007): 90–95. <https://doi.org/10/drbjhg>.
-   Waskom, M., Olga Botvinnik, Paul Hobson, John B. Cole, Yaroslav Halchenko, Stephan Hoyer, Alistair Miles, Tom Augspurger, Tal Yarkoni, Tobias Megies, Luis Pedro Coelho, Daniel Wehner, cynddl, Erik Ziegler, diego0020, Yury V. Zaytsev, Travis Hoppe, Skipper Seabold, Phillip Cloud, … Dan Allan. (2014). seaborn: v0.5.0 (November 2014). Zenodo. doi: 10.5281/zenodo.12710


## Environment

Dependencies (Packages installed) can be found in `requirements.txt` (conda list in `requirements_final.txt`). Installed via conda (see setup `conda_info.txt`) and pip.
