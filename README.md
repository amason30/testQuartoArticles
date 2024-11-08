
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

The differences between articles and vignettes, and where they are
stored (vignettes/articles vs. vignettes), have caused [issues with
pkgdown finding the rendered article
pages](https://github.com/r-lib/pkgdown/issues/2733). [Ethan
Bass](https://github.com/ethanbass) shows the issue is linked to a
discrepancy between where quarto is rendering the articles vs. where
pkgdown is searching for them when `build_quarto_articles()` is called
by pkgdown. I would like to note that Ethan created the [modified
code](https://github.com/ethanbass/pkgdown) to make this workflow work,
this repository is just my personal notes in implementing his fix!
Please see the GitHub issue linked above for more infomation in this
issue and Ethan’s [patched
pkgdown](https://github.com/ethanbass/pkgdown) for the code behind the
fix!

To get started, see [Quarto
articles](https://amason30.github.io/testQuartoArticles/articles/quarto-article1.html)
