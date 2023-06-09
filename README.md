# Population Autokorrelated Kernel Density Estimate (PKDE)

MoveApps

Github repository: https://github.com/ctmm-initiative/ctmmMoveApp_akdepop

## Description
Calculate mean home-range size, the joint home-range of the sample of tracked animals (=distribution of samples) and the population home range.

## Documentation
The app starts with a calculated autocorrelated kernel density estimates for several animals and then calculates a population mean home-range size, the joint home-range of the sample and the population home-range (utility distributions = UD).

Please see details of the Populaiton-level Autokorrelated Kernel Density Estimation in the help files of the functions within the ctmm R package: [akde](https://ctmm-initiative.github.io/ctmm/reference/akde.html) and [meta](https://ctmm-initiative.github.io/ctmm/reference/meta.html). 

### Input data
`ctmm UD with Data and Model` including the aKDE UD for all tracks

### Output data
`ctmm UD with Data and Model` including the pKDE UD and aKDE UDs for all tracks

### Artefacts

`akdepop_summary.pdf`: A figure of individual home-range areas at the 95 % isopleth and the mean of all individuals. 

`akdepop_summary.csv`: A summary of the of the mean home-range area (as returned by the function `ctmm::meta()`), the mean home-range area of the sample and the estimated home-range of the population (as returned by the `pkde()`-function). 

- `dist_of_sample_and_pop.pdf`: A plot of the distribution of samples (i.e. the tracked animals) and the distribution of the population home range (i.e., the population home-range as infered from the sample) as map. 

- `dist_pop.gpkg`: A geopackage of the population home range at the 95 % isopleth. 

- `dist_pop.tif`: The utilization distribution (UD) of the population home range.

- `dist_sample.gpkg`: A geopackage of the sample home range at the 95 % isopleth. 

- `dist_sample.tif`: The utilization distribution (UD) of the sample home range.

### Settings 
none

### Most common errors
Please issue an issue [here](https://github.com/ctmm-initiative/ctmmMoveApp_akdepop/issues) if you repeatedly encounter a specific error.

### Null or error handling
none at the moment
