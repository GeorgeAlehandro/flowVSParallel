# flowVSParallel

`flowVSParallel` is a modified version of the `flowVS` package, designed to perform variance stabilizing transformations on flow cytometry data. The key difference is that `flowVSParallel` is designed to run in parallel, which can significantly speed up computations for large datasets or many channels.

## Installation

To install `flowVSParallel`, you can use the `devtools` package in R. If you don't have `devtools` installed, you can install it with:

```r
install.packages("devtools")
devtools::install_github("GeorgeAlehandro/flowVSParallel")
```

## Usage
After installing flowVSParallel, you can load it in your R script with:

```r
library(flowVSParallel)
```
You can then use the estParamFlowVSParallel function to estimate the optimum parameters for variance stabilization in your flow cytometry data. See the documentation for estParamFlowVS for more information.

## Credits
All credits to the creator of the original package <a href="https://github.com/azadcse/flowVS">Ariful Azad</a> and <a href="https://bmcbioinformatics.biomedcentral.com/articles/10.1186/s12859-016-1083-9">the original paper</a>.
