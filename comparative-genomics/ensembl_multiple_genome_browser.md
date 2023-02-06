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
    + **Region Comparison**: it allows to compare a region between different species and the current species, including the visualization of custom data for each of these species. The comparisons are pair-wise compared to the current species.

* Genetic Variation:

    + Variant table:
    + Resequencing:
    + Strain table:

* ...

In the browser windows shown in each tab of the menu, we can configure the visualized tracks by clicking the *Add/remove tracks* button.

## Compare regions

Once in the browser, click **Region Comparison** in the left menu.

To select the desired species:

1. Click **Select species or regions**
2. Select the *Division* of the species (e.g. *rodents* > *rats and mice* > desired species)
3. Select the desired species (e.g. Ryukyu mouse, Shrew mouse, ...) and click **Apply**.

In the main window, different browsers will appear:

* The top one will show the region being compared in all the selected species and surrounding regions, without entering into much detail. 
* The bottom one (the interesting one) will show the alignment of the region being compared (red rectangle in the top browser). 

In the bottom browser, we will se the alignments of the region being compared in different assemblies. The comparisons will be pairwise between all the species and the current species. This means that:

* if two species are selected, the current species will appear on the middle of these two species. 
* if more than two species are selected, the track of the current species (e.g., GRCm39) will be duplicated, triplicated, etc, to show the alignment with all the species. (The regions are the same, so they can be removed from the exported image if necesseary). 

The interesting thing here is that we can **upload and visualiuze custom data**:

1. Click at the **Add/remove tracks** button (in the bottom browser).
2. Select the **Species to configure**.
3. Click at **Custom tracks** at the left menu or the **Personal data** at the top menú:

    + If not data from the selected species is uploaded, the window to upload the data will appear.
    + If data from the selected species is uploaded, a list of the uploaded tracks will appear. Click **Add new data** to go to the *uploading window*

4. In the window to add custom tracks, either:

    + Copy and paste the desired data to the text box, select the format of the data and click **Add data**
    + Upload the file with the desired data, select its format (e.g., Bedgraph, Bigwig...) and click **Add data**

5. Repeat the process for all the species shown.
6. Explore the desired regions.

For each custom track, the **max. size is 20MB**, so in most cases we will have to subset the data.

