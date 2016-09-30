
<!-- README.md is generated from README.Rmd. Please edit that file -->
This package contains datasets extracted from [OurWorldInData.org](https://ourworldindata.org): "an online publication that shows how living conditions around the world are changing". These data sets have undergone tidying so that they are suited to immediate analysis in R. The purpose of this package is to serve as a central R resource for thesedata sets so that they might be used for the likes of practice or exploratory data analysis in a replicable manner.

Considerable thanks must go to [Max Roser](http://www.maxroser.com/about/) and the rest of the [OurWorldInData team](https://ourworldindata.org/about/), who collate the datasets that are included in this package. If you appreciate their work and make use of this package, please consider supporting [OurWorldInData](https://ourworldindata.org/support/).

Data sets included in this package:
===================================

Population
----------

-   `child_mortality` Country-level changes in child mortality rates and related variables over time. A combination of all data sets available at <https://ourworldindata.org/child-mortality>.

Contributing to the ourworldindata R Package
============================================

Contributing to this package necessarily involves adding a data object to be exported with the package, and documentation that explains the data and variables. Ideally, an R file that shows how the data was compiled will also be included. These additions should appear as the following:

-   `data/NAME-OF-DATA.rda` which is the data object to be exported with the package.
-   `R/NAME-OF-DATA.R` which contains the roxygen comments that describe the data and each variable, and provide a link to the data source.
-   `R/data_prep/NAME-OF-DATA_prep.R` which is an R script that demonstrates how the data was compiled. These files will be ignored in the package build.

In addition to these files, any raw data files that were downlaoded and merged should also be saved into `data/raw_downloads`, which is ignored in the package build. This means that the raw data that contributed towards the final data object can be examined, and the timestamp for the commit means that the data version (e.g., if certain data sets are altered) can be tracked.
