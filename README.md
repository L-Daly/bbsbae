
<!-- badges: start -->
[![R-CMD-check](https://github.com/bbsBayes/bbsBayes2/actions/workflows/R-CMD-check.yaml/badge.svg)](https://github.com/bbsBayes/bbsBayes2/actions/workflows/R-CMD-check.yaml)
[![Codecov test coverage](https://codecov.io/gh/bbsBayes/bbsBayes2/branch/main/graph/badge.svg)](https://app.codecov.io/gh/bbsBayes/bbsBayes2?branch=main)
[![R-Universe](https://bbsbayes.r-universe.dev/badges/bbsBayes2)](https://bbsbayes.r-universe.dev/)
[![Project Status: Active](https://www.repostatus.org/badges/latest/active.svg)](https://www.repostatus.org/#active)

<!-- badges: end -->

# bbsBayes2 <img src="man/figures/logo.png" align="right"/>

bbsBayes2 is a package for performing hierarchical Bayesian analysis of North
American Breeding Bird Survey (BBS) data. 'bbsBayes2' will run a full model
analysis for one or more species that you choose, or you can take more control
and specify how the data should be stratified, prepared for Stan, or modelled.

Installation instructions are below.

See the [documentation](https://bbsbayes.github.io/bbsBayes2/articles/bbsBayes2.html) for an overview of
how to use bbsBayes2.

Additional resources:

* [Introductory bbsBayes Workshop]
* [Journal Article with worked example](https://doi.org/10.5334/jors.329)

## Installation

bbsBayes2 can be installed from the bbsBayes R-Universe:

```r
install.packages("bbsBayes2",
                 repos = c(bbsbayes = 'https://bbsbayes.r-universe.dev',
                           CRAN = 'https://cloud.r-project.org'))
```

Alternatively you can install directly from our GitHub repository with either
the [pak](https://pak.r-lib.org/) (recommended) or 
[remotes](https://remotes.r-lib.org/) packages.

With pak:

```{r}
install.packages("pak")
pak::pkg_install("bbsBayes/bbsBayes2")
```

With remotes:

```{r}
install.packages("remotes")
remotes::install_github(("bbsBayes/bbsBayes2")
```

If you want to install a developmental branch (at your own risk!), you can use 
the following (assuming you want to install a branch called `dev`).

```{r}
pak::pkg_install("bbsBayes/bbsBayes2@dev")
