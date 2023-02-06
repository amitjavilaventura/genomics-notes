# Genome Browsers

Genomic browsers are useful to visualize genomic data, ether public or custom data uploaded to the desired browser, but they have some limitations.

## _One-Genome_ Brosers

Most common browsers are:

- UCSC Genome Browser (online): https://genome.ucsc.edu/
- Inegrative Genomics Viewer (IGV) (standalone/online): https://igv.org/
- ENSEMBL Browser
- NCBI Browser
- VISTA Enhancer Browser

However, as far as I know, these browsers are limited to visualizing one genome per session, so making figures to compare different genomes (including genes, repeats, or gene expression tracks, etc) is difficult and usually renders less pretty figures. 

## Multiple Genome Browsers

To adress the issue of visualizing different genomes there are some browsers that allow to visualize multiple genomes:

* [*Multiple Genome Viewer* (MGV)](http://www.informatics.jax.org/mgv/), from the Mouse Genome Informatics (MGI):
 
   + Allows visualization of syntenic regions, including the gene annotations, from several mouse strains and species, as well as other model organisms.
   + Is limited to gene annotations, so it does not include repeats or regulatory elements. 
   + Does not allow to upload custom data, such as "bigwig" or "bed" files. 

* [`gggenes` R package](https://github.com/wilkox/gggenes/):

   + Very useful to visualize gene "structures" across different genomes using ggplots.
   + Limitations: only one gene annotation track (as far as I know);  cannot (or I don't know how to) use custom data (e.g. Bigwigs)

* [`gggenomes` R package](https://github.com/thackl/gggenomes): 

   + Very useful to draw browser-like ggplots comparing genes and orthology of multiple genomes. 
   + Limitations: only one gene annotation track (as far as I know);  cannot (or I don't know how to) use custom data (e.g. Bigwigs)

* [ENSEMBL Browser]():

   + explained `ensembl_multiple_genome_browser.md`.
