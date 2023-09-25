# Singularity for UBCG

Singularity recipe for [UBCG (Up-to-date Bacterial Core Genes)](http://leb.snu.ac.kr/ubcg2).

# Installation

Clone this repository, put the files from UBCG (UBCG.jar, programPath, UBCG.hmm) in the cloned folder together with the `ubcg.def`  and use the following command to create the singularity container:

```sudo singularity build ubcg.sif ubcg.def```

# Use

Call UBCG from the singularity using the command line:

```singularity exec ubcg2.sif java -jar /programs/UBCG.jar extract -i input_genome_fasta_file -bcg_dir output_ubcg_folder -label organism_name```
