--- 
title: "ComplexHeatmap Complete Reference"
author: "Zuguang Gu"
date: "last revised on 2020-04-29"
site: bookdown::bookdown_site
output: bookdown::gitbook
documentclass: book
bibliography: [book.bib]
biblio-style: apalike
link-citations: yes
github-repo: jokergoo/ComplexHeatmap-reference
cover-image: complexheatmap-cover.jpg
url: 'https\://jokergoo.github.io/ComplexHeatmap-reference/book'
description: "Complex heatmaps are efficient to visualize associations between different sources of data sets and reveal potential patterns. Here the ComplexHeatmap R package provides a highly flexible way to arrange multiple heatmaps and supports various annotation graphics. This book is the complete reference to ComplexHeatmap pacakge."
---

# About {-}

This is the documentation of the
[**ComplexHeatmap**](https://github.com/jokergoo/ComplexHeatmap) package. Examples in the book
are generated under version 2.5.1.

You can get a stable Bioconductor version from http://bioconductor.org/packages/release/bioc/html/ComplexHeatmap.html, but the most up-to-date version is always on Github and you can install it by:


```r
library(devtools)
install_github("jokergoo/ComplexHeatmap")
```

The [development branch on Bioconductor](http://bioconductor.org/packages/devel/bioc/html/ComplexHeatmap.html) is
basically synchronized to Github repository. 

The **ComplexHeatmap** package is inspired from the [**pheatmap**](https://CRAN.R-project.org/package=pheatmap) package. You can find many arguments in **ComplexHeatmap** have the same names as in **pheatmap**. Also you
can find [this old package](https://github.com/jokergoo/pheatmap2) that I tried to develop by modifying **pheatmap**.

**Please note, this documentation is not completely compatible with older versions (< 1.99.0, before
Oct, 2018), but the major functionality keeps the same.**

If you use **ComplexHeatmap** in your publications, I am appreciated if you can cite:

Gu, Z. (2016) Complex heatmaps reveal patterns and correlations in multidimensional genomic data.
DOI: [10.1093/bioinformatics/btw313](https://doi.org/10.1093/bioinformatics/btw313)


<img src="complexheatmap-cover.jpg" style="width:500px;border:2px solid black;" />



Session info:


```r
sessionInfo()
```

```
## R version 4.0.0 (2020-04-24)
## Platform: x86_64-apple-darwin17.0 (64-bit)
## Running under: macOS Catalina 10.15.4
## 
## Matrix products: default
## BLAS:   /Library/Frameworks/R.framework/Versions/4.0/Resources/lib/libRblas.dylib
## LAPACK: /Library/Frameworks/R.framework/Versions/4.0/Resources/lib/libRlapack.dylib
## 
## locale:
## [1] en_GB.UTF-8/en_GB.UTF-8/en_GB.UTF-8/C/en_GB.UTF-8/en_GB.UTF-8
## 
## attached base packages:
## [1] grid      stats     graphics  grDevices utils     datasets  methods  
## [8] base     
## 
## other attached packages:
## [1] dendsort_0.3.3       dendextend_1.13.4    circlize_0.4.9      
## [4] ComplexHeatmap_2.5.1
## 
## loaded via a namespace (and not attached):
##  [1] Rcpp_1.0.4.6        compiler_4.0.0      pillar_1.4.3       
##  [4] RColorBrewer_1.1-2  viridis_0.5.1       tools_4.0.0        
##  [7] digest_0.6.25       evaluate_0.14       lifecycle_0.2.0    
## [10] tibble_3.0.1        gtable_0.3.0        clue_0.3-57        
## [13] viridisLite_0.3.0   pkgconfig_2.0.3     png_0.1-7          
## [16] rlang_0.4.5         yaml_2.2.1          parallel_4.0.0     
## [19] xfun_0.13           gridExtra_2.3       stringr_1.4.0      
## [22] dplyr_0.8.5         cluster_2.1.0       knitr_1.28         
## [25] GlobalOptions_0.1.1 vctrs_0.2.4         tidyselect_1.0.0   
## [28] glue_1.4.0          R6_2.4.1            GetoptLong_0.1.8   
## [31] rmarkdown_2.1       bookdown_0.18       ggplot2_3.3.0      
## [34] purrr_0.3.4         magrittr_1.5        htmltools_0.4.0    
## [37] scales_1.1.0        ellipsis_0.3.0      assertthat_0.2.1   
## [40] shape_1.4.4         colorspace_1.4-1    stringi_1.4.6      
## [43] munsell_0.5.0       crayon_1.3.4        rjson_0.2.20
```

