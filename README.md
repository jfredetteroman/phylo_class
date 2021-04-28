# Phylogenetics Project: Start of Reproducible Script and To-Do List
Repository for botany 563 phylogenetics project

# Step 0: Install software

## Alignment software: T-Coffee

Using a Unix/Linux system, download the T-Coffee installer:

`wget http://tcoffee.org/Packages/Stable/Latest/ `

Grant execution permission to the installer:

`chmod +x T-COFFEE_installer_Version_13.45.0.4846264_linux_x64.bin`

Launch the installation wizard:

`./T-COFFEE_installer_Version_13.45.0.4846264_linux_x64.bin`

After following the installation wizard and restarting the terminal, verify that the installation was successful:

`t_coffee -version`

## Tree construction software: IQ-TREE

## Using this github repository alongside your analysis

Much of the data collection and sequence translation was completed outside of the command line due to limitations of certain tools and simplicity. While this readme still describes those steps in an effort to ensure reproducibility, those who wish to follow along starting with "Step 2: Multiple sequence alignment" should use the FASTA files included in this repository. In order to access these FASTA files (and the rest of the files included in this analysis), run the following git command:

`git clone https://github.com/jfredetteroman/phylo_project.git`

# Step 1: Collect Sequences

## BLAST Searches

Using the [species list](https://github.com/jfredetteroman/phylo_project/blob/main/SpeciesList.md) included in this repository and the genome database specified in the list, run a BLAST search on all species against the [*E. affinis* sequence](https://github.com/jfredetteroman/phylo_project/blob/main/FASTAs/Eurytemora_affinis_BLAST_reference.fa) included in this repository. For each BLAST result with an E-value smaller than 0.01, add the resulting sequence to a FASTA file corresponding to that species. The results from this step can be found in the [FASTAs](https://github.com/jfredetteroman/phylo_project/tree/main/FASTAs) directory.

## Convert to Amino Acid Sequences

Using [ExPASy's translate tool](https://web.expasy.org/translate/), convert nucleotide sequences for each species to amino acid sequences.

## Create FASTA file

Add each amino acid sequence to a FASTA file. To save time, the resulting FASTA file has been included in this repository.

# To-Do List--Remaining Steps

## Sequence Alignment

Install TM-Coffee

## Tree Estimation

Install IQ-TREE
