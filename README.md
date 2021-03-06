# dnaseq_analysis
Packages, tips etc for analysis of WEX/WGS/Amplicon sequencing data



# read/write genomic data

## reading in VCF data:

### [vcfR](https://github.com/knausb/vcfR)

VcfR is built upon two data structures.

vcfR - S4 class to contain data from a VCF file.

chromR - S4 class to contain variant information (VCF) and optional sequence (FASTA) and annotation (GFF) information.

Functions in vcfR provide the ability to subset VCF data as well as to extract and parse the data. For example, individual genotypes, sequence depths or genotype likelihoods (when provided in the VCF file) can easily be accessed. These tools are provided to aid researchers in rapidly surveying the quality and other characteristics of data provided as VCF data. With this information in hand, researchers should be able to determine criteria for hard filtering in order to attempt to maximize biological variation and minimize technical variation.

### [bedr](https://cran.r-project.org/web/packages/bedr/index.html)

Genomic regions processing using open-source command line tools such as 'BEDTools', 'BEDOPS' and 'Tabix'. These tools offer scalable and efficient utilities to perform genome arithmetic e.g indexing, formatting and merging. bedr API enhances access to these tools as well as offers additional utilities for genomic regions processing.

### [gwasvcf](https://github.com/MRCIEU/gwasvcf)

a wrapper around the bioconductor/VariantAnnotation package, providing functions tailored to GWAS VCF for reading, querying, creating and writing GWAS VCF format files
some LD related functions such as using a reference panel to extract proxies, create LD matrices and perform LD clumping
functions for harmonising a dataset against the reference genome and creating GWAS VCF files.

### [varikondo](https://annaquaglieri16.github.io/varikondo/index.html)

developed by the need to standardise and combine variant calling outputs from several callers as well as to allow an easy way to join filtering variants called from multiple samples within a patient.

Variants from different callers can be imported in R and parsed into a data frame with standardised fields. See how fields are standardaised to know more about which fields from each callers are parsed. The import functions are:



