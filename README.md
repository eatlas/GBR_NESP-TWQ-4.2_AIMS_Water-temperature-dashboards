# Oceanographic drivers of bleaching in the GBR: Water temperature dashboards (NESP TWQ 4.2, AIMS)

This code was used to generate the water temperature dashboards found on this
[temperature logger dashboards map](https://maps.eatlas.org.au/index.html?z=6&ll=147.90662,-16.53127&l0=ea_nesp4%3AGBR_AIMS_NESP-TWQ-4-2_Temp-Logger-Metadata_2015-17,ea_ea-be%3AWorld_Bright-Earth-e-Atlas-basemap,google_HYBRID,google_TERRAIN,google_SATELLITE,google_ROADMAP&v0=,,f,f,f,f&intro=false).

For more information, refer to the [eAtlas metadata record](https://eatlas.org.au/data/uuid/5dcde66c-0289-42e7-a833-c4cae065a213)

## Installation

The code is written in R. It requires the R binaries to interpret the code.
You can install R from the [R Project website](https://www.r-project.org/).

It also requires some external R libraries which can be install
using the `install_packages.R` script provided.

On Linux, you can execute it using the following command line:

```sudo ./install_packages.R```

## Input data

The data needed to generate the dashboard pages is not provided. It can be sourced
from https://www.aims.gov.au/docs/data/data.html
and https://www.qld.gov.au/environment/coasts-waterways/beach/monitoring/waves-sites

The input files need to be copied into its dedicated sub-folder in the `data` folder.

For more information, contact [Eduardo Klein Salas](eklein@ocean-analytics.com.au).

## Code execution

The R-Markdown code is executed using the `rmarkdown::render` method.

Example:

```R -e "rmarkdown::render('moorings_storyboard.Rmd',output_file='moorings_storyboard.html')"```
