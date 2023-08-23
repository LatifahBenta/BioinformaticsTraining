# QC ENVIRONMENT CODES

Herein are the commands used to ***create a new environment*** and ***install packages inside the environment**

***Base*** before the prompt tells us that we are using CONDA :+1:

### Creating a new environment.

We want to create an environment called **QC**.

The command to use to create this new environment is ***$ conda create -n qc***

### Confirming our current environment

It is good practice to confirm our current working environment.

We use the command ***$ conda env list*** 

base                  *  /home/administrator/miniconda3

new_env                  /home/administrator/miniconda3/envs/new_env

prokka                   /home/administrator/miniconda3/envs/prokka

qc                       /home/administrator/miniconda3/envs/qc

The *Asteriks* shows you your current working environment. In our case we are currently at the base.

### Switching environments

We want to install some packages in our new environment. We first move from the base to qc which is the name of our new environment .

The command to use is ***$ Conda activate qc***

We can confirm this has worked by listing our environments and confirming where the asteriks is
# conda environments:
#
base                     /home/administrator/miniconda3


new_env                  /home/administrator/miniconda3/envs/new_env

prokka                   /home/administrator/miniconda3/envs/prokka


qc                    *  /home/administrator/miniconda3/envs/qc

👏 👏 👏 Our current environment is qc.

### Installing packages.

We want to install the packages Fastqc and Multiqc in the qc environment

We start with **Fastqc** 

The command to use is ***$ conda install Fastqc***

We use the same command to install multiqc ***$ conda install Multiqc***

 **Proceed with y**
### Confirming our packages. 
We use the command ***$conda list*** to confirm if our packages are within the environment.

**We are all set now** :+1:


