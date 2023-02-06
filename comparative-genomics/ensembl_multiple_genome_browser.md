# Genome Browsers

Genomic browsers are useful to visualize genomic data, ether public or custom data uploaded to the desired browser, but they have some limitations.

## Limitations

**_One-Genome_ Brosers**

Most common browsers are:

- UCSC Genome Browser (online): https://genome.ucsc.edu/
- Inegrative Genomics Viewer (IGV) (standalone/online): https://igv.org/

However, as far as I know, these browsers are limited to visualizing one genome per session, so making figures to compare different genomes (including genes, repeats, or gene expression tracks, etc) is difficult and usually renders less pretty figures. 

**Multiple Genome Browsers**

To adress the issue of visualizing different genomes there are some browsers that allow to visualize multiple genomes, such as the [*Multiple Genome Viewer* (MGV)](http://www.informatics.jax.org/mgv/), from the Mouse Genome Informatics (MGI):
 
* Allows visualization of syntenic regions, including the gene annotations, from several mouse strains and species, as well as other model organisms.
* Is limited to gene annotations, so it does not include repeats or regulatory elements. 
* Does not allow to upload custom data, such as "bigwig" or "bed" files. 

# ENSEMBL Genome Browser

The [ENSEMBL Browser](http://www.ensembl.org/index.html) has all the ENSEMBL data available, which means:

* Data from ENSEMBL Compara, such as pairwise LastZ alignements, allows to visualize several genomes, including the syntenic regions.
* Annotations from Genecode ara available, so it is possible to visualize gene annotations.
* RepeatMasker (and other) tracks are available, so it is possible to visualize repeats.
* ...

Furthermore, the ENSEMBL Browser has the option to upload data in different formats (up to 20MB), including BigWig, BED, BedGraph.

Nevertheless, it is quite difficult, specially if the aim is to visualize several genomes including custom data. For this reason, I decided to write a "tutorial" to use it and don't forget how to use it. 

## Select the genome

Go te the ENSEMBL web site: http://www.ensembl.org/index.html

Select the genome you want to study (have in mind that it will be the assembly corresponding to the last ENSEMBL release): 

* In the "Favorite Genomes" genomes section, such as mouse *GRCm39/mm39* or human *GRCh38/hg38*.
* In unfoldable "Genomes" tab.

Once the genome has been selected (I selected the mouse *GRCm39*), several options will appear (e.g., **Search** genes, look at the **Genome assembly**, do **Comparative genomics**, ...)

## Explore the browser

To go to the browser, either *Search* a gene or click to *Example region*.

In the left menu, there are a lot of features to display in the genome (**Local-based displays**). Each of them may change a little based how the broser has opened and which tracks are loaded:

* Whole genome: shows all the chromosomes, and may show the localization of custom data if loaded.
* Chromosome summary: shows the current chromosome with the frequency of genes, non coding genes, repeats, etc. in each location.
* Region overview: shows a browser snapshot of the current region.
* Region in detail: shows a browser snapshot of the current region with more detail.
* **Comparative Genomics**

    + Synteny: shows the synteny of a chromosome between the current species and another one.
    + Alignments (image): shows the alignment of the current region between the current species and others, depening on the selected species in the multiple alignment (e.g., 21 murinae EPO). It includes the synteny of the regions between species.
    + Alignments (text): similar as *Aligments (image)* but with text and less detail.
    + **Region Comparison**: it allows to compare a region between different species and the current species, including the visualization of custom data for each of these species.

* Genetic Variation:

    + Variant table:
    + Resequencing:
    + Strain table:

* ...

## Compare regions

Once in the browser, click **Region Comparison** in the left menu.


