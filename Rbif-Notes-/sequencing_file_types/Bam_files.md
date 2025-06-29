# Bam files 

A SAM file (Sequence Alignment/Map) is a widely used text format in bioinformatics 
for storing large nucleotide sequence alignments. It’s the output of alignment 
tools like BWA, Bowtie2, or STAR when aligning sequencing reads to a reference genome.
this referenced sequence could be get from ncbi.

## creatign sam files:
Use the command bowtie2 -x index_genome.fasta -U <reads.fasQ> -S <output.sam>
** index_genome.fasta ** index file used by Bowtie 2 as an index files,
** reads.fastQ** is the input read file (e.g., a FASTQ file)
** output.sam ** is the desired name for the output SAM file