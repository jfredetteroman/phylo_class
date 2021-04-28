# Phylogenetics Project: Start of Reproducible Script and To-Do List
Repository for botany 563 phylogenetics project

# Step 1: Collect Sequences

## BLAST Searches

Using the species list included in this repository and the genome database specified in the list (SpeciesList.md), run a BLAST search on all species against the *E. affinis* sequence included in this repository (Eurytemora_affinis_BLAST_reference.fa). For each BLAST result with an E-value smaller than 0.01, add the resulting sequence to a FASTA file corresponding to that species. The results from this step can be found in the [FASTAs](https://github.com/jfredetteroman/phylo_project/tree/main/FASTAs) directory.

## Convert to Amino Acid Sequences

Using ExPASy's translate tool (https://web.expasy.org/translate/), convert nucleotide sequences for each species to amino acid sequences.

## Create FASTA file

Add each amino acid sequence to a FASTA file. To save time, the resulting FASTA file has been included in this repository.

# To-Do List--Remaining Steps

## Sequence Alignment

Install TM-Coffee

## Tree Estimation

Install IQ-TREE
