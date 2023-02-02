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

## First steps

Go te the ENSEMBL web site: http://www.ensembl.org/index.html

Select the genome you want to study (have in mind that it will be the assembly corresponding to the last ENSEMBL release). You can choose: 

* One of genomes in the "Favorite Genomes" genomes section, such as mouse *GRCm39/mm39* or human *GRCh38/hg38*.
* One of the genomes in the unfoldable "Genomes" tab and select the desired species.

Once the genome has been selected (I selected the mouse *GRCm39*), several options will appear (e.g., **Search** genes, look at the **Genome assembly**, do **Comparative genomics**. 

![]()
