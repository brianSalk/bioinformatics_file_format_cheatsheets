# fasta format
simple format stores one or more nucleic acid or protein sequnces.  
```
>sequence_name
SEQUNCE
```
## example
```
>chrom1
AATCACACACATATATGAGAGTAT
>chrome2
TTGTGTGTAAAGAGAACACGGTGTGTGTGGGGGGGCCCGG
>chrome3
TATATATATGGGGGGGGGGGTTATATATATATAGAGACCACACAC
```
## explaination
the name of each sequnce follows the '>' symbole.  
the next line(s) contain the sequence associated with the sequence name.  
## special nucleic acid characters
most of the time, DNA will only contain A,C,G, and T or U.  
Sometimes however, you will find the following characters:  
**N**: can represesnt any character  
**lowercase characters**: soft masked portions of the sequence.  These sequences were masked for lacking complexity.  

