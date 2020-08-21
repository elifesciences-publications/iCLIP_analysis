This code is associated with the paper from Mikedis et al., "DAZL mediates a broad translational program regulating expansion and differentiation of spermatogonial progenitors". eLife, 2020. http://doi.org/10.7554/eLife.56523

# iCLIP_analysis
Bash, python, and R scripts used to process and analyze iCLIP data. 

converting_mapped_reads_to_crosslinked_sites.py converts a sam file of mapped reads to a sam file of crosslinked positions (defined as the nucleotide immediately 5' to the 5' end of the mapped read). 

from_raw_sequencing_data_to_ASPeak.sh takes raw iCLIP sequencing data, quality trims, collapses PCR duplicates, demultiplexes, trims barcodes, aligns reads via STAR, converts mapped reads to crosslinked sites, and calls peaks using crosslinked sites via ASPeak. 

post_ASPeak_analysis.sh takes ASPeak output and identifies crosslinked sites, carries out motif analysis (HOMER, MEME, AME, kpLogo, and metaplot around crosslinked site), and analyzes conservation of crosslinked sites. 
