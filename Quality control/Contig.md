Originally ***contigs*** were defined by Staden as a set of gel readings that are related to one another by overlap of their sequences.

A **Contig** is a set of overlapping DNA segments that together represent a Consensus region of DNA.
A contig is a contiguous length of genomic sequence in which the order of bases is known to a high confidence level. 

***Consensus region of DNA*** is a calculated sequence of most frequent residues, either nucleotide or amino acids, found at each position in a sequence alignment.

In **Bottom-up** sequencing, a contig refers to overlapping sequence data.

The Bottom-up strategy consists of the following key steps:


- ***DNA Shearing***- Amplified Dna is randomly fragmented into appropriately sized pieces for sequencing.
-  ***DNA Assembly***- The subsequent sequence reads, data taht contain the sequences of the small fragments, are put into a database. The assembly software then searches the database for pairs of overlapping reads.

Assembling the reads from such a pair produces longer contiguous reads of sequenced DNA.

By repeating this process many times, at first with the initial pairs that are the result of previous assembly, the DNA sequence of an entire chromosome can be determined.

In ***Top-down/ Hierarchical*** Contig  refers to the overlapping clones that form a physical map of a chromosome.

In this sequencing method, a low-resolution map is made prior to sequencing in order to provide a framework to guide the later assembly of the sequence reads of the genome.

This map identifies the relative positions and overlap of the clones used for sequencing.
Sets of overlapping clones that form a contiguous stretch of DNA are called contigs; the minimum number of clones that form a contig that covers the entire chromosome comprise the tiling path that is used for sequencing.

Once a tiling path has been selected, its component BACs are sheared into smaller fragments and sequenced. Contigs therefore provide the framework for hierarchical sequencing.

The assembly of a contig map involves several steps.

- **DNA shearing** into larger (50–200kb) pieces, which are cloned into BACs or PACs to form a BAC library.
Since these clones should cover the entire genome/chromosome, it is theoretically possible to assemble a contig of BACs that covers the entire chromosome.


***Scaffolds*** is a portion of the genome sequence reconstructed from end-sequenced whole-genome shotgun clones.
Scaffolds are composed of contigs and gaps.

Gaps occur where reads from the two sequenced ends of at least one fragment overlap with other reads in two different contigs (as long as the arrangement is otherwise consistent with the contigs being adjacent). 
Since the lengths of the fragments are roughly known, the number of bases between contigs can be estimated. 

**N50** is a statistic that defines assembly quality in terms of Contiguity.

Given a set of contigs, the N50 is defined as the sequence length of the shortest contig at 50% of the total assembly length.

t can be thought of as the point of half of the mass of the distribution; the number of bases from all contigs longer than the N50 will be close to the number of bases from all contigs shorter than the N50

