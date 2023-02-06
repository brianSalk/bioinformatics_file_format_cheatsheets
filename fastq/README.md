# fastq format
```
@seq_name1
SEQUENCE
+
QUALITY_STRING
```
## Example
```
@read1
AACTGGAGAGATTAGAGAG
+
)ii++-232ii22k2k2k2
@read2
TTTTGGAAGAGATCCCCCC
+
2938298*(*292299999
```
## Explaination
the sequence name of the read precedes the '@'  
the actuall sequence is on the next line  
a plus sign seperates the sequence from the quality string.  
the quality string comes after the plus sign.  
repeat the above for each sequence you have.  
## Quality String:  
The quality string is a sequence of characters with ASCII values in the range \[33,126\] or characters in range \[!,~\]  
The higher the ASCII score, the higher chance that the read is correct.  
The probability that the read is correct is  
```math
10^{(-A/10)}$
```
Where $A$ is the ASCII value of the character in the quality string.
