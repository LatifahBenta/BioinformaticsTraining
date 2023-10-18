## Downloading a sequence

A number of databases that store biological data are available online: This include National Centre for Biotechnology Information (NCBI),European Molecular Biology Laboratory (EMBL), DNA Data Bank of Japan (DDBJ)

For this assignment i downloaded my sequence from **NCBI** 

Type NCBI on the Browser.

On the NCBI website page, navigate to the search bar, click the dropdown menu (*All databases*) and choose **SRA**.

Choose the Advanced settings that allows you to do a ***Boolean search***. This allows you to key in a string of characteristics in a single search.

My search string dor this search was **(Oxford Nanopore[Platform]) AND Bacteria[Organism]**

I settled on  the Accession number ***SRR26270940*** which is a sequence for *E.coli* and has a size of 2.6Mb and downloaded the Fastq format of the sequence.

The file downloaded is  **Gzip** file which is the standard file compression for Unix 

To decompress it we use the command `gunzip SRR26270940` 

Now you have a file that you can easily manipulate.😉

## Quality Control
Just like any other proceses, Quality Control is important in Bioinformatics for meaningful downstream analysis.

We created a new environment i called it **QC** .To create this environment I used the command `conda create -n QC`

In this environment we install **Fastqc** which provides a simple way to do some quality control checks on raw sequence data coming from High throughput sequencing pipelines.

Fastqc generates a report in an html format that enables you to spot problems originating either from the sequencer or the starting material for the library

I used the command `conda install -c Bioconda Fastqc` to install Fastqc within this environment.

To run fastqc on my sequence i used the command `Fastqc SRR26270940.fastq` and i got this report [Fastqc report](file:///home/administrator/Downloads/SRR26270940_fastqc.html)

Now lets assemble the sequence 😃

## FLYE

Flye is a ***de novo*** assembler for single molecule sequencing reads.

It is designed for a wide range of data sets, from small bacterial projects to large mammalian scale assemblers.

It takes in raw Pacbio or Oxford Nanopore technologies reads as inputs and outputs polished contigs.

I created a new environment called **Flye** using the command `conda create -n Flye` and activated it using the command `conda activate Flye`

In this environment i installed flye using the command `conda install -c bioconda Flye`

To assemble the sequence i used the command `flye --nano-raw SRR26270940.fastqc -o SRR26270940.fasta`

Our output is a **FASTA** file which is assembled.

Time to Visualize our data 🤝


