In this tutorial I checked the quality of FASTQ files to ensure that their data looks good before inferring any further information. This step is the usual first step for analyses such as RNA-Seq, ChIP-Seq, or any other OMIC analysis relying on NGS data. Quality control steps are similar for any type of sequencing data:

Quality assessment with tools like:
Short Reads:  FASTQE ( Galaxy version 0.3.1+galaxy0)
Short+Long:  FASTQC ( Galaxy version 0.73+galaxy0)
Long Reads:  Nanoplot ( Galaxy version 1.41.0+galaxy0)
Nanopore only:  PycoQC ( Galaxy version 2.5.2+galaxy0)
Trimming and filtering for short reads with a tool like Cutadapt
