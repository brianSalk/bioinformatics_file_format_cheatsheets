# fastq format
fastq format is similar to fasta format in that they both contain the name of a sequence along with the actuall sequence intself.  
The biggest difference is that fastq also contains a quality string.  
When Next Generation Sequencers (NGS) read DNA/protein sequences, they may make mistakes.  
In addition to reading the Base or Amino acid in a sequence, NGS also produce a quality score for each read.  
The quality score is expressed as a character who's ASCII value.  
The higher the ASCII value of the character, the higher certainty we have that the read is correct.  
Phred quality score:  
first convert the character to its ASCII score to get the Phred score.  
Then you can calculate the probability that the read at each position is an error by the following equation:  
$$
10^{(-\text{Phred}/10)}
$$
