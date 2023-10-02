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

## ParallelFlowVS Shiny App

A Shiny app for ParallelFlowVS, hosted in a Docker container for easy deployment and use.

### Getting Started

To get started, you'll need to have [Docker](https://www.docker.com/get-started) installed on your machine.

### Pulling the Docker Image

First, pull the latest version of the Docker image from Docker Hub by running the following command in your terminal:

```bash
docker pull georgealehandro/parallelflowvs_shiny:latest
```
### Launching the APP

Once you have pulled the Docker image, you can launch the Shiny app by running the following command:
```bash
docker run -d -p 7777:3838 georgealehandro/parallelflowvs_shiny:latest
```
Now, you should be able to access the Shiny app by navigating to http://localhost:7777 in your web browser.

(You can replace `7777` with any other available port number on your machine if needed.)


## Credits
All credits to the creator of the original package <a href="https://github.com/azadcse/flowVS">Ariful Azad</a> and <a href="https://bmcbioinformatics.biomedcentral.com/articles/10.1186/s12859-016-1083-9">the original paper</a>.
