Set-up
======

A local installation of R (version 4.1 or greater) is required before installing RStudio. Instructions may vary based on the OS you are using (Windows, MacOS, Linux etc.). Please follow instructions found here:
http://mixomics.org/wp-content/uploads/2016/09/Installation-guide-for-R-and-RStudio.pdf

Please install the following R packages through RStudio. Some dependency packages might be required for successful installation. 

**These packages can be installed by copying the R code into your RStudio console and running.**


code-block:: R

    # Create a directory to store workshop datasets and R code
    - this can be done by right clicking and selecting ‘New Folder’
    - Alternitively this can also be done within Rstudio, using the unix ‘Terminal’ - the tab next to ‘Console’
    ```bash
    mkdir -p ~/Documents/scrna-seq_workshop
    ````
    # copy datasets into working directory
    - links to the datasets are via the following one drive address,
    https://sahmrionline-my.sharepoint.com/:f:/g/personal/cathal_king_sahmri_com/EnnB7Iwxn25HtwACcTXD8ZkBr8YLjk61-FxGEPE-vPdLyQ?e=roceOt
    - click ‘Download’ and copy the data to the workshop directory, e.g. ~/Documents/scrna-seq_workshop
    # check the data
    ```bash
    cd ~/Documents/scrna-seq_workshop/
    ls -l
    #unzip if needed (can be done with a double cllick on a mac)
    unzip Workshop_scRNA-seq.zip
    open Workshop_scRNA-seq.zip   #mac
    ls -l          #unix
    ``
    # Within Rstudio, in set this directory as the working directory
    setwd(‘~/Documents/scrna-seq_workshop’)


.. code-block:: R

    # Seurat
    install.packages("Seurat")
    library(Seurat)

.. code-block:: R

    # SeuratObject
    install.packages("SeuratObject")
    library(SeuratObject)    

.. code-block:: R

    # Remotes
    install.packages("remotes")
    library(remotes)

.. code-block:: R
    
    # Install Seurat (version 5) alternative
    remotes::install_github("satijalab/seurat", "seurat5", quiet = TRUE)

.. code-block:: R

    # tidyverse
    install.packages("tidyverse")
    library(tidyverse)

.. code-block:: R

    # msigdbr
    install.packages("msigdbr")
    library(msigdbr)

.. code-block:: R

    # SoupX
    install.packages("SoupX")
    library(SoupX)

.. code-block:: R

    # dittoSeq
    if (!require("BiocManager", quietly = TRUE))
    install.packages("BiocManager")
    BiocManager::install("dittoSeq")
    library(dittoSeq)



More information about each package can be found below.

==========  =====
Package     URL      
==========  =====  
Seurat*     https://satijalab.org/seurat/
devtools*   https://www.r-project.org/nosvn/pandoc/devtools.html
ggplot2*    https://ggplot2.tidyverse.org/
cellchat*   https://github.com/sqjin/CellChat
dittoSeq    https://bioconductor.org/packages/release/bioc/html/dittoSeq.html
SoupX*      https://github.com/constantAmateur/SoupX
msigdbr*    https://cran.r-project.org/web/packages/msigdbr/vignettes/msigdbr-intro.html
==========  =====  
Test installation of each package using the ``library()`` function.


