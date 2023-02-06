# fastq format
```
@seq_name1
SEQUENCE
+
QUALITY_STRING
@seq_name2
SEQUNCE
+
QUALITY_STRING
```

## Quality String:  
The quality string is a sequence of characters with ASCII values in the range \[33,126\] or characters in range \[!,~\]  
The higher the ASCII score, the higher chance that the read is correct.  
```math
$10^{(-\text{Phred}/10)}$
```
