
<!-- README.md is generated from README.Rmd. Please edit that file -->

# testQuartoArticles

<!-- badges: start -->

[![pkgdown.yaml](https://github.com/amason30/testQuartoArticles/actions/workflows/pkgdown.yaml/badge.svg)](https://github.com/amason30/testQuartoArticles/actions/workflows/pkgdown.yaml)
[![pages-build-deployment](https://github.com/amason30/testQuartoArticles/actions/workflows/pages/pages-build-deployment/badge.svg)](https://github.com/amason30/testQuartoArticles/actions/workflows/pages/pages-build-deployment)
<!-- badges: end -->

This repository was created to test the ability of using quarto (.qmd)
files as articles for R packages when builing a website with pkgdown.
Further it shows how to ensure the website builds correctly when
deployed with GitHub actions.

As of version 2.1.1, pkgdown supports the [use of
quarto](https://pkgdown.r-lib.org/articles/quarto.html) vignettes. Yay!
This is awesome, quarto has so many great features and has awesome
extensions in VS code and other IDE’s. However, vignettes != articles.
Articles are often used by package developers to show documentation,
tutorials, etc. on a resource website for uses. The advantage of using
articles is clear for packages analyzing large datasets that you do not
want packaged with the package or extra dependencies that are only
needed to show data pipelines/integration of your package with other,
existing packages. The main difference between an article and vignette,
is an vignette is shipped with the package and an article is only
displayed on the package website. You can read more on the differences
in [Hadley’s R packages
book](https://r-pkgs.org/vignettes.html#sec-vignettes-article).

To get started, see [Quarto
articles](https://amason30.github.io/testQuartoArticles/articles/quarto-article1.html)
