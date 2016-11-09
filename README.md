The Leek group guide to genomics papers 
==============

When I was a student, my advisor [John Storey](http://www.genomine.org/) made a list of papers for me to read on nights and weekends. That list was incredibly helpful for a couple of reasons. 

* It got me caught up on the field of computational genomics
* It was expertly curated, so it filtered a lot of papers I didn't need to read
* It gave me my first set of ideas to try to pursue as I was reading the papers

I have often thought I should make a similar list for folks who may want to work wtih me (or who want to learn about statistical genomics). So this is my attempt at that list. I've tried to separate the papers into categories and I've probably missed important papers. I'm happy to take suggestions for the list, but this is primarily designed for people in my group so I might be a little bit parsimonious. 



Background on genomics
=====================

* [Molecular structure of nucleic acids: A structure for deoxyribose nucleic acid](http://www.nature.com/scitable/content/molecular-structure-of-nucleic-acids-a-structure-13997975) - the paper describing the structure of DNA. Was the very beginning of the genomics revolution. The authors won a Nobel Prize. They used data from [Rosalind Franklin](http://www.goodreads.com/book/show/326851.Rosalind_Franklin) to do it. 
* [Central dogma of molecular biology](http://www.nature.com/nature/focus/crick/pdf/crick227.pdf) - by one of the people who discovered the structure of DNA, outlines the main information flow from DNA to proteins (which then flow to phenotypes). 
* [Next-generation DNA sequencing](http://www.nature.com/nbt/journal/v26/n10/full/nbt1486.html) - introduces the main technology used today to measure DNA, RNA, protein-DNA binding, epigenetic marks like DNA methylation, chromatin folding, etc. 
* [Ultrafast and memory-efficient alignment of short DNA sequences to the human genome](http://genomebiology.com/2009/10/3/r25) - a paper describing a very fast way to align sequence reads to the genome. One of the first to do this. 
* [A gene expression barcode for microarray data](http://www.ncbi.nlm.nih.gov/pmc/articles/PMC3154617/) - a paper describing the way that genes are expressed ("turned on") or not expressed ("turned off") in microarray data. 

Background on RNA-seq
======================

* [RNA-Seq: a revolutionary tool for transcriptomics](http://www.nature.com/nrg/journal/v10/n1/full/nrg2484.html) - introduces RNA-sequencing, the main type of data we look at in the Leek group. 
* [Mapping and quantifying mammalian transcriptomes by RNA-seq](http://www.nature.com/nmeth/journal/v5/n7/abs/nmeth.1226.html) - introduces many of the key computational issues in RNA-seq analysis. 
* [From RNA-seq reads to differential expression results](http://genomebiology.com/2010/11/12/220) - probably the single best review of RNA-seq analysis written. 
* [IVT-seq reveals extreme bias in RNA sequencing](http://genomebiology.com/2014/15/6/R86) - an important paper showing potential sources of bias in RNA-seq analysis using experimental data. 





Background on Statistics
=========================

* [Sequencing technology does not eliminate biological variability](http://biostat.jhsph.edu/~jleek/papers/seqvar.pdf) - a paper describing the sources of variability in genomic experiments and the importance of different types of replicates.
* [Linear models and empirical bayes methods for assessing differential expression in microarray experiments.](http://www.ncbi.nlm.nih.gov/pubmed/16646809) - introduces a general linear modeling framework, including the most successful use of variance shrinkage to date. This is the first paper behind the [limma](http://www.bioconductor.org/packages/release/bioc/html/limma.html) package. 
* [Evaluation of statistical methods for normalization and differential expression in mRNA-Seq experiments](http://www.biomedcentral.com/1471-2105/11/94) - one of the first papers to describe basic statistical modeling for RNA-seq, covers many of the most important issues. 
* [voom: precision weights unlock linear model analysis tools for RNA-seq read counts](http://genomebiology.com/2014/15/2/R29) - updates the limma framework to sequencing experiments.
* [edgeR: a Bioconductor package for differential expression analysis of digital gene expression data](http://www.ncbi.nlm.nih.gov/pmc/articles/PMC2796818/) and [Differential expression of sequence count data](http://www.biomedcentral.com/content/pdf/gb-2010-11-10-r106.pdf) are papers on how to do differential expression using read counts, based on similar shrinkage ideas to those in limma. 
* [Statistical significance for genome-wide studies](http://www.pnas.org/content/100/16/9440.abstract) - introduces the basic concepts behind high-dimensional multiple testing and the false discovery rate in an approachable way. 
* [Tackling the widespread and critical impact of batch effects in high-throughput data](http://www.nature.com/nrg/journal/v11/n10/full/nrg2825.html) - talks about batch effects, one of the most common confounders in genomic studies, and how to address them; related software is the [sva package](http://www.bioconductor.org/packages/release/bioc/html/sva.html). There are other confounders as well, this paper: [http://www.plosgenetics.org/article/info%3Adoi%2F10.1371%2Fjournal.pgen.0030161](http://www.plosgenetics.org/article/info%3Adoi%2F10.1371%2Fjournal.pgen.0030161) talks about some of them. 
* [Statistical inferences for isoform expression in RNA-Seq](http://bioinformatics.oxfordjournals.org/content/25/8/1026.full.pdf) - a very useful paper for defining a model or isoform expression in RNA-seq. 
* [Gene set enrichment analysis made simple](http://www.ncbi.nlm.nih.gov/pubmed/20048385) - a paper describing a simple approach to identifying gene sets that are enriched for differential expression. 


Background on software
=====================

* [Tidy data](http://vita.had.co.nz/papers/tidy-data.pdf) - a paper where Hadley Wickham describes proper organization of data sets that I really like. 
* [The Leek group guide to data sharing](https://github.com/jtleek/datasharing) - how to organize data you are working on. 
* [Bioconductor: open software development for computational biology and bioinformatics](http://genomebiology.com/content/5/10/R80) - introduces the Bioconductor project, the most successful project in genomic software development to date. 
* [Scalable genomics with R and Bioconductor](http://arxiv.org/pdf/1409.2864v1.pdf) - how to do big genomics data in R using [Bioconductor](http://bioconductor.org/). 
* [The Leek group guide to writing R packages](https://github.com/jtleek/rpackages) - how to make R packages. 
* [Differential gene and transcript expression analysis of RNA-seq experiments with TopHat and Cufflinks](http://www.nature.com/nprot/journal/v7/n3/abs/nprot.2012.016.html) - protocols for using Cufflinks and Tophat, two commmon pieces of software we use. 

Papers from the Leek group you should read
=====================

Obviously [all of them](http://jtleek.com/papers/)

* [Sequencing technology does not eliminate biological variability](http://biostat.jhsph.edu/~jleek/papers/seqvar.pdf) - a paper describing the sources of variability in genomic experiments and the importance of different types of replicates.
* [Differential expression analysis of RNA-seq data at single-base resolution](http://biostatistics.oxfordjournals.org/content/early/2014/01/06/biostatistics.kxt053.short) - proposes a new approach to finding differentially expressed regions in the human genome. 
* [Flexible analysis of transcriptome assemblies with Ballgown](http://biorxiv.org/content/biorxiv/early/2014/09/05/003665.full.pdf) - describes a statistical backend for popular transcript assembly algorithms. 




A partial set of papers to round out your knowledge
=====================

* [PHYLOGENIES FROM MOLECULAR SEQUENCES: INFERENCE ANDRELIABILITY ](http://www.annualreviews.org/doi/pdf/10.1146/annurev.ge.22.120188.002513) - a slightly older review of phylogenetic inference by one of the real titans in the area. 
* [On Differential Variability of Expression Ratios: Improving Statistical Inference about Gene Expression Changes from Microarray Data](http://online.liebertpub.com/doi/abs/10.1089/106652701300099074) - probably the first real description of empirical bayes approaches for genomics data. 
* [The allelic architecture of human disease genes: common disease-common variant...or not?](http://www.ncbi.nlm.nih.gov/pubmed/12351577) - a discussion of whether common genetic variants lead to common diseases. 
* [Genetic Dissection of Transcriptional Regulation in Budding Yeast](http://www.sciencemag.org/content/296/5568/752.short) - the paper that launched the whole area of eQTL analysis which is really hot right now. 
* [Inference of population structure using multi-locus genotype data](http://www.genetics.org/content/155/2/945.long) - one of the most foundational papers on how we infer population structure. 
