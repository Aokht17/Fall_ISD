# Immunosuppressive domains in human genome  
Immunosuppressive domains (ISD) are usually short (about 20-40 amino acids) peptide sequences that have retroviral (and some other viruses’) origin or are similar to viral envelope glycoproteins and are able to interact with immune cells’ receptors leading to an inhibition of the response and immunosuppression. 

The studied immunosuppressive peptides are composed of two regions: active site (AS) and receptor-binding (R) site, and have middle loop formed by a disulfide bond. They also have a glycosylation site, which can be located both inside and outside the loop and which is important part of many membrane and secretory proteins. This cysteine loop and α-helixes are conservative structures and can be found in immunosuppressive domains of such common proteins as syncitins. 

It is known that retroviruses are able to integrate and stay in our genes for a long time (so-called endogenous retroviruses). ISD sequences can be found in approximately 8% of the human genome, and therefore they are interesting from a genetic and evolutionary point of view. What is more, specifically selected ISDs can be used in transplantology, in the treatment of autoimmune diseases. The understanding of mechanisms of action is closely related to the treatment of viral diseases.

## Aims of the project
The aim of the project was to find tissue-specific immunosuppressive domains in human genome using predicted artificial peptides from patent as a query template.

## Objectives
+ transcribe the reference human genome in 6 reading frames
+ search for similar protein sequences in the transcriptome using different tools
+ analyze received data, select coding sequences
+ evaluate the expression level in various tissues
+ select loci with tissue specificity 

## Materials and methods
To make a genome-wide search, two principal tools were used. We performed genome translation in 6 reading frames (3 forward and 3 reverse) using EMBOSS.6.6.0 and created local protein database. Then, a hidden Markov model of aligned amino acid sequences was created, which was used for search (HMMER-3.3). After that we launched local tblastn on the same data. We compared the obtained results and checked the differential expression using a GTEx database.

#### Tools and databases:
+ NCBI (*Homo sapiens* reference genome (assembly GRCh38.p13))
+ Emboss 6.6.0
+ mafft online
+ hmmer-3.3
+ local TBLASTN 2.6.0+
+ databases GTEx (mainly), IncRNA, UniProt

## Results
As a result, many unidentified loci were found, as well as non-coding RNAs. Among the detected protein products, the majority does not have tissue-specific expression. 
3 loci encoding tissue-specific peptides were identified:
| gene | location | tissue |
|:---------------------------|:----------------:|:---------------------------:|
|ERVW-1 (also known as HERV-W)| 7q21. 2| testis and placenta|
|ERVV-1 (also known as HERV-V1)|19q13.41 |kidney and some parts of the brain|
|ERVV-2 (HERV-V2)| 19q13.41 |kidney|

## References
Grandi, N., & Tramontano, E. (2018). *HERV Envelope Proteins: Physiological Role and Pathogenic Potential in Cancer and Autoimmunity*. Frontiers in Microbiology, 9.
Blinov, V. M., Krasnov, G. S., Shargunov, A. V., Shurdov, M. A., & Zverev, V. V. (2013). *Immunosuppressive domains of retroviruses: Cell mechanisms of the effect on the human immune system*. Molecular Biology, 47(5), 613–621.
Heidmann, O., Béguin, A., Paternina, J., Berthier, R., Deloger, M., Bawa, O., & Heidmann, T. (2017). *HEMO, an ancestral endogenous retroviral envelope protein shed in the blood of pregnant women and expressed in pluripotent stem cells and tumors. Proceedings of the National Academy of Sciences*, 114(32), E6642–E6651. 
Lonsdale et al. (2013). *The Genotype-Tissue Expression (GTEx) project*. Nature Genetics, 45(6), 580–585. 



