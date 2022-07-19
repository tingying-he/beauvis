# BeauVis: A Validated Scale for Measuring the Aesthetic Pleasure of Visual Representations

  

This is a repository for all data and analysis scripts used in the VIS 2022 paper "BeauVis: A Validated Scale for Measuring the Aesthetic Pleasure of Visual Representations".

## Requirements
The R script requires, in addition to a normal R installation, several packages including (potentially more):
* ``png``
* ``psych``
* ``EFA.dimensions``
* ``imager``
* ``corrplot``
* ``knitr``
* ``kableExtra``
* ``xtable``
* ``dplyr``
* ``tibble``
* ``ggplot2``
* ``lavaan``
* ``ltm``

To install required packages, run the following script:
``Rscript -e "install.packages(c('png', 'psych', 'EFA.dimensions', 'imager', 'corrplot', 'knitr', 'kableExtra', 'xtable', 'dplyr', 'tibble', 'ggplot2', 'lavaan', 'ltm'), repos='https://cran.rstudio.com')"``

## Running the script
1. clone this repository
2. knit the oneclick.Rmd by running
 `` Rscript -e 'library(rmarkdown); rmarkdown::render("/PathTo/oneclick.Rmd", "html_document")' ``

## Files produced
In the "results" folder, you can see the following figures and tables of this paper.
* Fig. 1, 3, 6, 8 - 23, 43 - 57
* Table 1 - 5, 12 - 56