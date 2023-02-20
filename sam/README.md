# sam format
A sam file starts with comments that are prefixed with '@'  
after the comments, there are rows of tab seperated values where each row is a mapping of a read to a reference genome.  
each row conrtains the following information.  

**1)** QNAME: Query template NAME, which is the read ID or name  
**2)** FLAG: bitwise FLAG indicating various attributes of the read and alignment  
**3)** RNAME: Reference sequence NAME, which is the name of the reference chromosome or contig to which the read was aligned  
**4)** POS: 1-based leftmost mapping POSition of the read on the reference  
**5)** MAPQ: MAPping Quality of the read, which is the phred-scaled probability that the alignment is incorrect  
**6)** CIGAR: CIGAR string describing how the read aligns to the reference  
**7)** RNEXT: Reference name of the mate/next read  
**8)** PNEXT: Position of the mate/next read  
**8)** TLEN: Observed Template LENgth, which is the inferred insert size (i.e., the distance between the 5' ends of the two reads in a paired-end   sequencing experiment)  
**8)** SEQ: segment SEQuence, which is the nucleotide sequence of the read  
**8)** QUAL: ASCII of base QUALity plus 33, which is the base quality scores of the read in phred scale  
