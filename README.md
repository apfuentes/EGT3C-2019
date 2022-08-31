# EGT3C-2019

> Instructor: Angela P. Fuentes-Pardo, PhD, Uppsala University, e-mail: apfuentesp@gmail.com

## 2019-11-19

### Objectives
- Become familiarized with R
- Learn how to perform population genomics analysis in R


### Table of contents
1. Basic statistics
   - Genetic diversity (Ho, He) - `R`

2. Population genetic structure
   - Pairwise FST - `R`
   - Unsupervised clustering (PCA, nMDS) - `R`
   - Model-based clustering - `ADMIXTURE`
   - Genotype x Environment Association (Redundancy Analysis, RDA) - `R`

### Programs and R packages required
-	[plink v1.9](http://zzz.bwh.harvard.edu/plink/)
- [PGDSpider](http://www.cmpg.unibe.ch/software/PGDSpider/)
-	[Admixture](http://software.genetics.ucla.edu/admixture/)
- [R](https://www.r-project.org)
- [Rstudio](https://rstudio.com)
- R packages:

```R
install.packages(c("ade4", "adegenet", "ape", "circlize", "ComplexHeatmap", "data.table", "devtools", "diveRsity", "dplyr", "gdistance", "genepopedit", "geosphere", "ggplot2", "ggpubr", "ggrepel", "ggsn", "gplots", "hierfstat", "igraph", "knitr", "lattice", "magrittr", "mapdata", "maps", "maptools", "marmap", "mmod", "pcadapt", "pegas", "pegas", "phangorn", "pinfsc50", "plyr", "poolfstat", "poppr", "psych", "qqman", "randomForest", "RColorBrewer", "RCurl", "reshape2", "rgdal", "rgeos", "rmatio", "Rmisc", "sp", "stringr", "tidyr", "tidyverse", "tools", "treemap", "vcfR", "vegan", "VennDiagram", "viridisLite"), repos = "http://cran.rstudio.com", dependencies = TRUE)

# If genepopedit is not available, install it.
if (!require("genepopedit")) {
  if (!require("devtools")) install.packages("devtools") # Install the R package devtools
  devtools::install_github("rystanley/genepopedit") # Install the package from *Github*
}
```

**Note:** You need to have `java JDK v1.8` and `python3` previously installed in your machine. If you are having problems installing some R packages (e.g. `devtools`), search in the internet for a solution. *Hint*: A system library might be missing in your machine.


### Data
- SNP genotype data (96 loci) of 1308 individuals from 27 locations (Lehnert et al.,2017). SNP panel of 96 SNPs generated from RAD-seq data of Wyngaarden et al. (2017)
- Environmental data of sampling locations

### References and other recommended readings:
- [Special issue in Molecular Ecology on Population Genomics in R](https://onlinelibrary.wiley.com/toc/17550998/17/1)
- [Lehnert et al. (2019) Fine-scale temperature-associated genetic structure between inshore and offshore populations of sea scallop (Placopecten magellanicus). Heredity 122:69–80](https://www.nature.com/articles/s41437-018-0087-9)
- [Wyngaarden et al. (2017) Identifying patterns of dispersal, connectivity and selection in the sea scallop, Placopecten magellanicus, using RADseq-derived SNPs. Evolutionary Applications 10:102–117](https://onlinelibrary.wiley.com/doi/10.1111/eva.12432)

