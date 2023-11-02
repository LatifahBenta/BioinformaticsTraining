## Downloading sequences

We were to download 5 E.coli sequences from **Sequence Reads Archive**

Go to the NCBI website

On the database dropdown arrow click on SRA and search

We can create a boolean search based on the type of sequences we want but, i just used the Organism class and keyed in *E.coli*then searched.

From this search I got the following sequences.


|Accession # |Size      |
|------------|----------|
|SRR23800501 | 542.9Mb  |
|SRR23044203 |	412.5Mb |
|SRR23044204 |	424.1Mb |
|SRR23044205 | 	424.8Mb |
|SRR23100674 | 359.1Mb   |


We would need to make the use of sra-tools which is a collection of tools and libraries for using data in the INSDC SRA

I first used the command `conda install -c bioconda sra-tools`

This command installed sra-tools in my system however when i tried to run the command `prefetch SRR5790106` // Prefetch not found

Prefetch is a command used to download all necessary files into your computer. It can be invoked multiple times if the download did not succeed and will pick up from the last invocation failed.

My error could be because this version of sra-tools had not been updated or the version of sra-tools was not compatible to my current linux system.

I then used the command `Conda uninstall sra-tools` to uninstall the package

I then used the command `conda create -y -n ncbi -c conda-forge -c bioconda -c defaults sratools=2.10.1 entrez-direct=13.9`

I got the same error as before. This time the problem was because the sratools i got was not updated. The command I used was to search for sra-tools in the channels starting with conda-forge which had a version that was not updated.

To uninstall i again used the command `conda uninstall sra-tools`

The Bioconda page which was last updated one month ago had the most updated version.

I created an environment that would house the sra-tools as well as its dependencies.

`conda create -n sra-tools` and used the command `conda activate sra-tools` to get into the environment to download the sra-toolkit package.

I used the command `conda -c bioconda sra-tools`

I then changed directories to Documents because that is where i waanted my sequences to be downloaded. `cd Documents`

To download my sequences i used the command ` prefetch SRR23800501 SRR23044203 SRR23044204 SRR23044205 SRR23100674`

After downloading we need to extract the files. For this we use the commands `fastq-dump` or `fasterq-dump` however `fasterq-dump` is much faster than `fastq-dump`

The command `fasterq-dump SRR23800501 SRR23044203 SRR23044204 SRR23044205 SRR23100674`

Now we have **.fastq** version of the sequences we had downloaded.







