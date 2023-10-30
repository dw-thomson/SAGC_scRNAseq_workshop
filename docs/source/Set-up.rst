Set-up
======

A local installation of R (version 4 or greater) is required before installing RStudio. Instructions may vary based on the OS you are using (Windows, MacOS, Linux etc.). Please follow instructions found here:
http://mixomics.org/wp-content/uploads/2016/09/Installation-guide-for-R-and-RStudio.pdf

Please install the following R packages through RStudio. Some dependency packages might be required for successful installation. These packages can be installed by copying the R code into your RStudio console and running.

.. code-block:: R

    install.packages(‘Seurat’)
    library(Seurat)

.. code-block:: R
    ## Install Seurat (Alternative)
    ## alternative method of installation
    remotes::install_github(“satijalab/seurat”, “seurat5”, quiet = TRUE)

.. code-block:: R

    install.packages(“tidyverse”)

.. code-block:: R


.. code-block:: R

.. code-block:: R

==========  =====
Package     URL      
==========  =====  
Seurat*     https://satijalab.org/seurat/
devtools*   https://www.r-project.org/nosvn/pandoc/devtools.html
ggplot2*    https://ggplot2.tidyverse.org/
cellchat*   https://github.com/sqjin/CellChat
dittoSeq    https://bioconductor.org/packages/release/bioc/html/dittoSeq.html
SoupX       https://github.com/constantAmateur/SoupX
msigdbr     https://cran.r-project.org/web/packages/msigdbr/vignettes/msigdbr-intro.html
==========  =====  
Test installation of each package using the ``library()`` function.


