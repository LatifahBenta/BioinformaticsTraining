# Downloading sequences

We were to download 5 *E.coli* sequences from **Sequence Reads Archive** 

Go to the NCBI website

On the database dropdown arrow click on SRA and search

We can create a boolean search based on the type of sequences we want but, i just used the Organism class and keyed in *E.coli*  then searched

We would need to make the use of **sra-tools** which is a collection of tools and libraries for using data in the INSDC SRA

I first used the command `conda install -c bioconda sra-tools`

This command installed sra-tools in my system however when i tried to run the command `prefetch SRR5790106` it gave an error #Prefetch not found

This could be  because this version of sra-tools had not been updated or the version of sra-tools was not compatible to my current linux system.

I then used the command `wget --output -document sratoolkit.tar.gz https://ftp-trace.ncbi.nlm.nih.gov/sra/sdk/current/sratoolkit`

I got an error in trying to untar the directory This is because the 



