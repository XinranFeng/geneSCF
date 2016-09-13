Gene Set Clustering based on Functional annotation
----------------------------------------------------------------------------

INSTALL:

No installation required

TEST DATASETS:

Run command

./test_geneSCF

You will get output in './test/output/' directory.


USAGE: 

geneSCF <OPTIONS> -i=<INPUT FILE> -o=<OUTPUT PATH/FOLDER> -db=<GO_all|GO_BP|GO_MF|GO_CC|KEGG|REACTOME|NCG>

==========
Options:
==========

[-i= | --infile=]	Input file contains list of Entrez GeneIDs or OFFICIAL GENE SYMBOLS.
			The genes must be new lines seperated (One gene per line).

[-t= | --gtype=]	Type of input in the provided list either Entrez GeneIDs 'gid'
			or OFFICIAL GENE SYMBOLS 'sym' (Without quotes, default: sym).

[-db= | --database=]	Database you want to find gene enrichment which is either 
			geneontology 'GO_all' or geneontology-biological_process 
			'GO_BP' or geneontology-molecular_function 'GO_MF' or 
			geneontology-cellular_components 'GO_CC' or kegg 'KEGG' or 
			reactome 'REACTOME' or Network of Cancer Genes 'NCG' (Without quotes).

[-o= | --outpath=]	Path to save output file. The output will be with saved in the 
			provided existing location as 
			{INPUT_FILE_NAME}_{database}_functional_classification.tsv 
			(tab-seperated file). Note: This tool will not create output directory, 
			only outputs in exiting location.

[-bg= | --background=]	Total background genes to consider (default : 30000).

[-h | --help]		For displaying this help page.



--------------------------
Cite using: 

Subhash S and Kanduri C. GeneSCF: a real-time based functional enrichment tool with support for multiple organisms. BMC Bioinformatics 2016, 17:365, http://www.biomedcentral.com/1471-2105/17/365


--------------------------
Author: Santhilal Subhash
santhilal.subhash@gu.se
Last Updated: 2015 June 05
