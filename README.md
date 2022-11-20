# EGEA
## Every Gene Ever Annotated in published GWAS

This is a public repository collecting the gene annotations Eric Fauman has contributed to various published GWAS

Specifically, these annotations come from the following three publications:

## Sources
1.	Stacey D, Fauman EB, Ziemek D, et al. 
*ProGeM: a framework for the prioritization of candidate causal genes at molecular quantitative trait loci*. Nucleic Acids Res. 2019;47(1):e3. 
doi:10.1093/nar/gky837

2.	Yin X, Chan LS, Bose D, et al. 
*Genome-wide association studies of metabolites in Finnish men identify disease-relevant loci*. Nat Commun. 2022;13(1):1644. Published 2022 Mar 28. 
doi:10.1038/s41467-022-29143-5

3.	Surendran P, Stewart ID, Au Yeung VPW, et al. 
*Rare and common genetic determinants of metabolic individuality and their effects on human health*. Nat Med. 2022;28(11):2321-2332. 
doi:10.1038/s41591-022-02046-0


## These are the specific tables used for each set of causal gene annotations:

1. https://pubmed.ncbi.nlm.nih.gov/30239796/
  
    - Stacey D, Fauman EB, Ziemek D, et al. 
    - **ProGeM: a framework for the prioritization of candidate causal genes at molecular quantitative trait loci.** 
    - Nucleic Acids Res. 2019;47(1):e3. 
    - doi:10.1093/nar/gky837
    - https://www.ncbi.nlm.nih.gov/pmc/articles/PMC6326795/bin/gky837_supplemental_files.zip
    - Table S1

2. https://pubmed.ncbi.nlm.nih.gov/35347128/

    - Yin X, Chan LS, Bose D, et al. 
    - **Genome-wide association studies of metabolites in Finnish men identify disease-relevant loci.** 
    - Nat Commun. 2022;13(1):1644. Published 2022 Mar 28. 
    - doi:10.1038/s41467-022-29143-5
    - https://www.ncbi.nlm.nih.gov/pmc/articles/PMC8960770/bin/41467_2022_29143_MOESM4_ESM.xlsx
    - Supplementary Data 3
    - Supplementary Data 7

3. https://pubmed.ncbi.nlm.nih.gov/36357675/

    - Surendran P, Stewart ID, Au Yeung VPW, et al. 
    - **Rare and common genetic determinants of metabolic individuality and their effects on human health.**
    - Nat Med. 2022;28(11):2321-2332. 
    - doi:10.1038/s41591-022-02046-0
    - https://static-content.springer.com/esm/art%3A10.1038%2Fs41591-022-02046-0/MediaObjects/41591_2022_2046_MOESM2_ESM.xlsx
    - Supplementary Table 7

## Summary Table

In each of the 3 papers above I specifically annotated a SNP-metabolite pair with one or more causal genes. In cases like the FADS1|FADS2 locus I explicitly annotated the association with the pair because biochemistry along can't uniquely identify the causal gene (for most metabolites).
I collected the smallest p-value for any metabolite assigned to each particular causal gene across the 3 papers.
The attached file, egea_met.txt, lists one entry for each causal gene, or set of nearby causal genes (e.g., FADS1|FADS2), representing the strongest metabolite (or metabolite ratio) association at that locus.
The column headers are:
1. gene - Eric Fauman's annotation as to the causal gene at the locus. If more than one gene is listed it means I can't ascertain a unique causal gene because the paralogs at the locus have similar functions. But I am fairly certain that the true causal gene is one (or more) of the listed genes
2. nlp - the -log10(p) of the strongest association assigned to the gene/locus across the 3 publications
3. trait - the name of the metabolite (or metabolite ratio) with the smallest p-value at the locus
4. rsid - the rsid of the sentinel or lead SNP
5. explanation - the biochemical rational for my selection of the causal gene, as reported in one of the 3 papers
6. explanation_source - the pubmedid of the original functional/experimental work linking the gene to the metabolite
7. gwas_source - the pubmedid of the GWAS generating the p-value for this SNP and this metabolite
8. annotation_source - the pubmedid containing the original causal gene annotation (one of the 3 papers listed above)

