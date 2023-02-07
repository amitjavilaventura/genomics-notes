# Splicing efficiency

## 1. Read mapping

To study splicing, it is important to use a **splice-aware aligner** to map the reads, such as [`STAR`](https://physiology.med.cornell.edu/faculty/skrabanek/lab/angsd/lecture_notes/STARmanual.pdf), [`Hisat2`](http://daehwankimlab.github.io/hisat2/manual/) or [`TopHat`](https://ccb.jhu.edu/software/tophat/manual.shtml). 

These read aligners, usually require a splice site annotation. However, many times, we want them to discover not annotated splicing events.


