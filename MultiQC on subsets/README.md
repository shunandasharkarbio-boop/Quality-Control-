With paired-end sequencing, the fragments are sequenced from both sides. This approach results in two reads per fragment, with the first read in forward orientation and the second read in reverse-complement orientation. With this technique, we have the advantage to get more information about each DNA fragment compared to reads sequenced by only single-end sequencing:

    ------>                       [single-end]

    ----------------------------- [fragment]

    ------>               <------ [paired-end]
The distance between both reads is known and therefore is additional information that can improve read mapping.

Paired-end sequencing generates 2 FASTQ files:

One file with the sequences corresponding to forward orientation of all the fragments
One file with the sequences corresponding to reverse orientation of all the fragments
Usually we recognize these two files which belong to one sample by the name which has the same identifier for the reads but a different extension, e.g. sampleA_R1.fastq for the forward reads and sampleA_R2.fastq for the reverse reads. It can also be _f or _1 for the forward reads and _r or _2 for the reverse reads.

The data we analyzed in the previous step was single-end data so we will import a paired-end RNA-seq dataset to use. We will run FastQC and aggregate the two reports with MultiQC Ewels et al. 2016.
