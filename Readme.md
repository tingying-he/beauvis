# BeauVis: A Validated Scale for Measuring the Aesthetic Pleasure of Visual Representations

This is a repository for all data and analysis scripts used in the paper "[BeauVis: A Validated Scale for Measuring the Aesthetic Pleasure of Visual Representations](https://doi.org/10.1109/TVCG.2022.3209390)", presented at [IEEE Visualization 2022](http://ieeevis.org/year/2022/welcome) and published in the journal [IEEE Transactions on Visualization and Computer Graphics](https://ieeexplore.ieee.org/xpl/RecentIssue.jsp?punumber=2945). If you use the results in new projects or use it in a different way we would appreciate a citation:

Tingying He, Petra Isenberg, Raimund Dachselt, and Tobias Isenberg. BeauVis: A Validated Scale for Measuring the Aesthetic Pleasure of Visual Representations. IEEE Transactions on Visualization and Computer Graphics, 2023. To appear. doi: [10.1109/TVCG.2022.3209390](https://doi.org/10.1109/TVCG.2022.3209390); open-access versions are available at https://hal.inria.fr/hal-03763559 and at https://doi.org/10.48550/arXiv.2207.14147

## Bibtex
```
@article{He:2023:BVS,
  author      = {Tingying He and Petra Isenberg and Raimund Dachselt and Tobias Isenberg},
  title       = {{B}eau{V}is: A Validated Scale for Measuring the Aesthetic Pleasure of Visual Representations},
  journal     = {IEEE Transactions on Visualization and Computer Graphics},
  year        = {2023},
  volume      = {29},
  number      = {1},
  month       = jan,
  pages       = {363--373},
  doi         = {10.1109/TVCG.2022.3209390},
  doi_url     = {https://doi.org/10.1109/TVCG.2022.3209390},
  oa_hal_url  = {https://hal.inria.fr/hal-03763559},
  preprint    = {https://doi.org/10.48550/arXiv.2207.14147},
  osf_url     = {https://osf.io/fxs76/},
  osf_url2    = {https://osf.io/djrn3/},
  url         = {https://tobias.isenberg.cc/VideosAndDemos/He2023BVS},
  url2        = {[https://www.aviz.fr/Research/BeauVis-Scale](https://tingying-he.github.io/projects/He_2023_BeauVis.html)},
  url3        = {https://www.aviz.fr/Research/BeauVis-Scale},
  github_url  = {https://github.com/tingying-he/beauvis},
  pdf         = {https://tobias.isenberg.cc/personal/papers/He_2023_BVS.pdf},
}
```

## Project websites
* https://tobias.isenberg.cc/VideosAndDemos/He2023BVS
* https://tingying-he.github.io/projects/He_2023_BeauVis.html
* https://www.aviz.fr/Research/BeauVis-Scale

## Requirements

The R script contained within this repository requires, in addition to a [normal R installation](https://cran.r-project.org/), several packages including (potentially more):
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

To install these required packages, run the following call from a command line:
``Rscript -e "install.packages(c('png', 'psych', 'EFA.dimensions', 'imager', 'corrplot', 'knitr', 'kableExtra', 'xtable', 'dplyr', 'tibble', 'ggplot2', 'lavaan', 'ltm'), repos='https://cran.rstudio.com')"``

If you encounter problem with Pandoc:
1. To check whether Pandoc was correctly installed: ``Rscript -e "rmarkdown::pandoc_exec()"``
2. To install Pandoc from its official website: https://pandoc.org/installing.html . If you use macOS, you can also use Homebrew to install it: ``brew install pandoc``

## Running the R script
1. clone this repository ``git clone git@github.com:tingying-he/beauvis.git`` or downlaod codes through zip from the repository
2. change to the cloned directory ``cd beauvis``
3. knit the ``oneclick.Rmd`` by running `` Rscript -e "library(rmarkdown); rmarkdown::render('./oneclick.Rmd', 'html_document')" ``
## Files produced
After the script completes, in the ``results`` folder you should see the following figures and tables [from the paper](https://tobias.isenberg.cc/personal/papers/He_2023_BVS.pdf):
* Fig. 3 (``ScreePlot-Image_1 .pdf``)
* Fig. 6a (``Image 2  Ratings Per Scale.pdf``)
* Fig. 6b (``Image 9  Ratings Per Scale.pdf``)
* Fig. 8 (``Average Rating for the 5 item scale.pdf``)
* Fig. 9–23 (``ScreePlot-Image_* .pdf``)
* Fig. 43–57 (``Image *  Ratings Per Scale.pdf``)
* Table 1 (``factor_numbers.tsv``)
* Table 2 (``cfa_good_fit.tsv``)
* Table 3 (``cfa_factor_loading.tsv``)
* Table 4 (``cfa_alpha.tsv``)
* Table 5 (``cfa_pearson.tsv``)
* Tables 12–26 (``efa_1factor_image*.tsv``)
* Tables 27, 29, 31, 33, 35, 37, 39, 41, 43, 45, 47, 49, 51, 53, 55 (``efa_2factors_varimax_image*.tsv``)
* Tables 28, 30, 32, 34, 36, 38, 40, 42, 44, 46, 48, 50, 52, 54, 56 (``efa_2factors_promax_image*.tsv``)

Other images from the paper (i.e., Fig. 5, Fig. 24–27, Fig. 28–42) were created with the tool [Tableau](https://www.tableau.com/), so we could not script them.
