# Basic Local Alignment Search Tool

BLAST finds regions of similarities between Biological Sequences.
 It compares proteins or nucleotide sequences to sequence databases and calculates the statistical significance.

 BLAST has different flavors depending on the type of sequence you have and the database you want to run your sequence against.

 ### Flavors of BLAST.

 **BLASTn** -Compares a Nucleotide sequence against a Nucleotide database

 **BLASTp** - Compares a Protein Sequence to a Protein database.

 **BLASTx**-Translates nucleotide sequences in all six reading frames and compares them to protein databases. Great for finding protein-coding regions in DNA.

 **tBLASTn**: Compares protein sequences to translated nucleotide databases. Useful when you want to find nucleotide sequences that code for a given protein.

**tBLASTx**: Translates both the query and database sequences and then compares them. This can be useful for finding distant relationships.

**psiBLAST**: Stands for Position-Specific Iterated BLAST. It's an iterative version of BLASTp that refines the search based on the results of previous searches.

**PHI-BLAST**: Stands for Pattern-Hit Initiated BLAST. It's specialized for searching for short, nearly exact matches to a pattern within a sequence database.

**DELTA-BLAST**: Designed to find distant evolutionary relationships between proteins. It uses a more sensitive search strategy.
