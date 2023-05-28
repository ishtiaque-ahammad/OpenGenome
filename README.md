# OpenGenome
OpenGenome is an easy-to-use multi-modal genome assembly tool that performs quality control, genome assembly, removal of unassembled contigs and provides a summary of the assembled genome (length of the genome, number of contigs, minimum and maximum length of the contigs, n50, n75, n90 statistics etc). If allows the users to choose trimmers (trimmomatic/ fastp) as well as assemblers (megahit/ spades/ unicycler) through a simple prompt. Users can get their genome assembled and polished after quality control and also get important statistics regarding the genome just by providing the raw read file names, name of the trimmer and the assembler to use, and the number of cpu core they want to use for the analysis at the beginning. 
# Installation
If Conda package management software is not already installed on your computer, download and install it from the official Conda website (https://docs.conda.io/en/latest/miniconda.html).
## Step 1:
Download the OpenGenome script file and the OpenGenome.yml file in your computer and navigate to that directory.

## Step 2:
Move the OpenGenome script file to /usr/local/bin/ using the following command:

sudo mv OpenGenome /usr/local/bin/

## Step 3: 
Create the OpenGenome environment using the following command:

conda env create -n OpenGenome -f OpenGenome.yml
# Usage
## Step 1: 
Activate the OpenGenome environment using the following command:

conda activate OpenGenome
## Step 2: 
Run the following command:

OpenGenome

OpenGenome will ask you to provide the following things:

1.The name of the raw sequencing files i.e. forward and reverse read files

2.Choice of assembler (megahit / spades/ unicycler)

3.The number of CPU cores you want to use

After you provide the neccessary info, it will start running!
## Input
OpenGenome takes in raw sequencing data (paired end) in .fastq format.
## Output
Once OpenGenome is finished running, the output files will be available in the OpenGenome_Output folder.
