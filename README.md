# 182-project
## Files
1. reference.fasta -- the reference SARS-CoV-2 genome from https://www.ncbi.nlm.nih.gov/nuccore/NC_045512
2. annotation.gff -- the annotation file from the cov2-site https://www.ncbi.nlm.nih.gov/sars-cov-2/
3. full_accession.txt -- the accession list from the cov2-site https://www.ncbi.nlm.nih.gov/sars-cov-2/
4. accession.txt -- our list of accession numbers extracted from full_accession.txt, starting at the 2401 th and ending at the 2500 th accession number
5. sequence.fasta -- complete record of the nucleotide sequences corresponding to our accession numbers from Genbank https://www.ncbi.nlm.nih.gov/sites/batchentrez
6. CodingSeqProtein.txt -- Fasta formatted database of SARS-CoV-2 proteins (downloaded from NCBI). Note1: this is the protein sequence, not nucleotide sequence. Note2: some information may need to be added to the headers manually / by program base on annotation.gff. Don't use it yet.
7. CodingSeqProteinAnnoHeader.txt -- Fasta formatted database of SARS-CoV-2 proteins protein coding sequence with header replaced by annotation attributes
8. blastx_e-40.txt -- blastx output using CodingSeqProteinAnnoHeader.txt as database and sequence.txt as query sequence and evalue of 1e-40.
9. blastx_e-5.txt -- blastx output using CodingSeqProteinAnnoHeader.txt as database and sequence.txt as query sequence and evalue of 1e-5.
10. blastx_e-30.txt -- blastx output using CodingSeqProteinAnnoHeader.txt as database and sequence.txt as query sequence and evalue of 1e-30.
11. mutation_hunt_combined.ipynb -- Jupyter notebook that does the mutation hunt
12. MutationHuntRes.txt -- output of mutation_hunt_combined.ipynb. Format: Mutation:frequencency. Sorted.
