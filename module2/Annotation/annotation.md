Step 1)
Filtering contigs shorter than 500 bp.
Tool: Filter FASTA 
Version: Galaxy Version 2.3
Parameters: Filtered on sequence length; min. length 500 bp

Step 2)
Quality assessment using CheckM2
Tool: CheckM2
Version: Galaxy Version 1.1.0 + galaxy0
Parameters: Model Options - Output quality prediction for both models for each genome

Step 3)
Genome annotation
Tool: Prokka
Version: Galaxy Version 1.14.6 + galaxy1
Parameters: Force GenBank compliance - Yes

Step 4)
Species ID
Tool: BLAST
Version: BLASTn (web)
Parameters: rRNA/ITS database

Step 5)
Build phylogenetic tree
Tool: Type Strain Genome Server 
Version: https://tygs.dsmz.de/ (web)
Parameters: Whole Proteome Tree

Step 6)
Visualize phylogenetic tree
Tool: Interactive Tree of Life
Version: ITOL version 7 (web)
Parameters: Display bootstraps as text

Step 7)
Average nucleotide identity
Tool: ezbiocloud.net
Version: I don't know not listed (web)
Parameters: From NCBI Genome Database, downloaded the FASTA file for Salmonella Typhimurium (closest hit on 16s blast) and Salmonella bongori (more distant relative). Compared filteredFasta.fasta to the fasta files from typhimurium and S. bongori.