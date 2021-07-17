# GENE-ANALYSIS 

## ABOUT
Small project developed to test several Biopython modules by analysing genes. The main aim is to automatise the whole process of gathering information about genes and proteins and analyse them. 
For this project the example selected was the cell line OV90 from ovarian cells. This cell line is widely used in studies regarding ovarian cancer, one of the most agressive forms of cancer in females. The expression of STX4, STXBP3 and SNAP29 genes might have a correlation with the development of ovarian cancer. Resorting to bioinformatic tools makes the analysis of this correlation easier, thus facilitating the understanding of the metabolism of OV90 cancer cells in order to find potential drug targets that may help treating this disease.

## Prerequisites

In order to properly execute this program, it is necessary to install the Biopython package.

``` pip install biopython ```

## Usage
The classes developed in ``` OV90.py ``` where created in order to retrieve gene information from online databases such as NCBI and analysing it using several tools available in Biopython. 

``` OV90.py ``` contains the following classes:

- ``` Search ``` : searches for useful literature and articles that may help understand the information retrieved from a certain gene.
- ``` RetrieveInfo ```: retrieves the gene file from NCBI and filters the information contained within it.
- ``` Blast ```: performs a _blastn_ program in order to find homologous sequences to the one being analized.
- ``` Align ```: performs alignments of either one or two+ sequences.
- ``` Clustal ```: performs multiple sequence alignment using clustalw.
- ``` Phylo ```: displays a phylogenetic tree.
- ``` SearchP ```: searches for protein information in protein related databases.
- ``` ProteinBlast ```: performs a _blastp_ program given a protein query.

To test them, a test script ``` OV90_run.py ``` was created. So far, not all classes are implemented within ```OV90_run.py```. 
As an example, the gene __STX4__ was used to test out the program. 

