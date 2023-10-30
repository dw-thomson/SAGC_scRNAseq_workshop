Set-up
======

A local installation of R (version 4 or greater) is required before installing RStudio. Instructions may vary based on the OS you are using (Windows, MacOS, Linux etc.). Please follow instructions found here:
http://mixomics.org/wp-content/uploads/2016/09/Installation-guide-for-R-and-RStudio.pdf

Please install the following R packages through RStudio. Some dependency packages might be required for successful installation. These packages can be installed by copying the R code into your RStudio console and running.

.. code-block:: R

    install.packages(‘Seurat’)
    library(Seurat)

.. code-block:: R
    ## Install Seurat (version 5)
    remotes::install_github(“satijalab/seurat”, “seurat5”, quiet = TRUE)

.. code-block:: R

    install.packages(“tidyverse”)

.. code-block:: R

    install.packages(“msigdbr”)
    library(msigdbr)

.. code-block:: R

    install.packages(‘SoupX’)
    library(SoupX)

.. code-block:: R

    if (!require(“BiocManager”, quietly = TRUE))
    install.packages(“BiocManager”)
    BiocManager::install(“dittoSeq”)
    library(dittoSeq)

.. code-block:: R

    ## Install Seurat
    * required
    ```{Install Seurat_Cran}
    # Enter commands in R (or R studio, if installed)
    install.packages(‘Seurat’)
    library(Seurat)
    ```
    ## Install Seurat (Alternative)
    * alternative method of installation
    ```{Install Seurat_remotes}
    remotes::install_github(“satijalab/seurat”, “seurat5”, quiet = TRUE)
    ```
    ## Install tidyverse
    ```{Install tidyverse}
    install.packages(“tidyverse”)
    ```
    ## Install msigdbr
    ```{Install msigdbr}
    install.packages(“msigdbr”)
    library(msigdbr)
    ```
    ## Install SoupX
    ```{Install SoupX}
    install.packages(‘SoupX’)
    library(SoupX)
    ```
    ## Install dittoSeq
    ```{Install dittoSeq}
    if (!require(“BiocManager”, quietly = TRUE))
        install.packages(“BiocManager”)
    BiocManager::install(“dittoSeq”)
    library(dittoSeq)
    ```
    ### I think we should remove the following if possible
    ## Install SingleCellExperiment
    ```{Install SingleCellExperiment}
    if (!require(“BiocManager”, quietly = TRUE))
        install.packages(“BiocManager”)
    BiocManager::install(“SingleCellExperiment”)
    library(SingleCellExperiment)
    ```

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


