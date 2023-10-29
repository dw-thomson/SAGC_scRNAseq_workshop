Set-up
======

A local installation of R (version 4 or greater) is required before installing RStudio. Instructions may vary based on the OS you are using (Windows, MacOS, Linux etc.). Please follow instructions found here:
http://mixomics.org/wp-content/uploads/2016/09/Installation-guide-for-R-and-RStudio.pdf

Please install the following R packages in your current RStudio session. Some might require other dependency packages that should be installed upon installation.

==========  =====
Package     URL      
==========  =====  
Seurat      https://satijalab.org/seurat/
scater      https://bioconductor.org/packages/release/bioc/html/scater.html
SCE	        https://bioconductor.org/packages/release/bioc/html/SingleCellExperiment.html
tidyverse   https://www.tidyverse.org/
scran       https://bioconductor.org/packages/release/bioc/html/scran.html
cellchat    https://github.com/sqjin/CellChat
scRNAseq    https://bioconductor.org/packages/release/data/experiment/html/scRNAseq.html
msigdbr     https://cran.r-project.org/web/packages/msigdbr/vignettes/msigdbr-intro.html
cellula     https://gdagstn.github.io/cellulaweb/install.html
==========  =====  
Test
====
Once packages are installed, test installation using the library function.
.. code-block:: R
   library(cellchat)


