The Leek group guide to genomics papers (WARNING: WORK IN PROGRESS!!!!)
==============

When I was a student, my advisor [John Storey](http://www.genomine.org/) made a list of papers for me to read on nights and weekends. That list was incredibly helpful for a couple of reasons. 

* It got me caught up on the field of computational genomics
* It was expertly curated, so it filtered a lot of papers I didn't need to read
* It gave me my first set of ideas to try to pursue as I was reading the papers

I have often thought I should make a similar list for folks who may want to work wtih me (or who want to learn about statistial genomics). So this is my attempt at that list. I've tried to separate the papers into categories and I've probably missed important papers. I'm happy to take suggestions for the list, but this is primarily designed for people in my group so I might be a little bit parsimonious. 



Background on genomics
=====================

* [Molecular structure of nucleic acids: A structure for deoxyribose nucleic acid](http://www.nature.com/scitable/content/molecular-structure-of-nucleic-acids-a-structure-13997975) - the paper describing the structure of DNA. Was the very beginning of the genomics revolution. The authors won a Nobel Prize. They used data from [Rosalind Franklin](http://www.goodreads.com/book/show/326851.Rosalind_Franklin) to do it. 
* [Central dogma of molecular biology](http://www.nature.com/nature/focus/crick/pdf/crick227.pdf) - by one of the people who discovered the structure of DNA, outlines the main information flow from DNA to proteins (which then flow to phenotypes). 
* [Next-generation DNA sequencing](http://www.nature.com/nbt/journal/v26/n10/full/nbt1486.html) - introduces the main technology used today to measure DNA, RNA, protein-DNA binding, epigenetic marks like DNA methylation, chromatin folding, etc. 
* [Ultrafast and memory-efficient alignment of short DNA sequences to the human genome](http://genomebiology.com/2009/10/3/r25) - a paper describing a very fast way to align sequence reads to the genome. One of the first to do this. 
* 

Background on RNA-seq
======================

* [RNA-Seq: a revolutionary tool for transcriptomics](http://www.nature.com/nrg/journal/v10/n1/full/nrg2484.html) - introduces RNA-sequencing, the main type of data we look at in the Leek group. 
* [Mapping and quantifying mammalian transcriptomes by RNA-seq](http://www.nature.com/nmeth/journal/v5/n7/abs/nmeth.1226.html) - introduces many of the key computational issues in RNA-seq analysis. 
* [A gene expression barcode for microarray data](http://www.ncbi.nlm.nih.gov/pmc/articles/PMC3154617/) - a paper describing the way that genes are expressed ("turned on") or not expressed ("turned off") in microarray data. 
* [From RNA-seq reads to differential expression results](http://genomebiology.com/2010/11/12/220) - probably the single best review of RNA-seq analysis written. 


Background on Statistics
=========================

* [Linear models and empirical bayes methods for assessing differential expression in microarray experiments.](http://www.ncbi.nlm.nih.gov/pubmed/16646809) - introduces a general linear modeling framework, including the most successful use of variance shrinkage to date. This is the first paper behind the [limma](http://www.bioconductor.org/packages/release/bioc/html/limma.html) package. 
* [Statistical significance for genome-wide studies](http://www.pnas.org/content/100/16/9440.abstract) - introduces the basic concepts behind high-dimensional multiple testing and the false discovery rate in an approachable way. 
* 


Background on software
=====================

* [Tidy data](http://vita.had.co.nz/papers/tidy-data.pdf) - a paper where Hadley Wickham describes proper organization of data sets that I really like. 
* [The Leek group guide to data sharing](https://github.com/jtleek/datasharing) - how to organize data you are working on. 
* [Scalable genomics with R and Bioconductor](http://arxiv.org/pdf/1409.2864v1.pdf) - how to do big genomics data in R using [Bioconductor](http://bioconductor.org/). 
