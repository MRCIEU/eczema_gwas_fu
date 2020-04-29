## Preparation of LD reference panel data
**1000 Genomes EUR. Generate haploblocks with gpart and bigLD**
```
sh ./bayesian_fm/ref_panel/01_1kGenomes_ref_panel.sh)
```
[https://github.com/MRCIEU/eczema_gwas_fu/blob/master/bayesian_fm/ref_panel/01_1kGenomes_ref_panel.sh](https://github.com/MRCIEU/eczema_gwas_fu/blob/master/bayesian_fm/ref_panel/01_1kGenomes_ref_panel.sh)

**UK Biobank EUR**
```
sh ./bayesian_fm/ref_panel/02_ukbiobank_ref_panel.sh)
```
[https://github.com/MRCIEU/eczema_gwas_fu/blob/master/bayesian_fm/ref_panel/02_ukbiobank_ref_panel.sh](https://github.com/MRCIEU/eczema_gwas_fu/blob/master/bayesian_fm/ref_panel/02_ukbiobank_ref_panel.sh)

## Define LD-based interval GWAS lead SNPs
```
sh ./colocalization/coloc/05_coloc_analysis_r2_p_interval.sh)
```
[https://github.com/MRCIEU/eczema_gwas_fu/blob/master/colocalization/coloc/05_coloc_analysis_r2_p_interval.sh](https://github.com/MRCIEU/eczema_gwas_fu/blob/master/colocalization/coloc/05_coloc_analysis_r2_p_interval.sh)

## Annotation and subsetting of datasets used in GWAS fine-mapping analysis
```
sh ./annotation/data_manipulation/01_data_cleanup.sh
```
[https://github.com/MRCIEU/eczema_gwas_fu/blob/master/annotation/data_manipulation/01_data_cleanup.sh](https://github.com/MRCIEU/eczema_gwas_fu/blob/master/annotation/data_manipulation/01_data_cleanup.sh)

## Individual analyses - gene based

**CEDAR eQTL identification and colocalisation with coloc**
```
sh ./analysis/cedar/01_cedar_ciseqtl_gemma_r2_p_interval.sh
```
[https://github.com/MRCIEU/eczema_gwas_fu/blob/master/analysis/cedar/01_cedar_ciseqtl_gemma_r2_p_interval.sh](https://github.com/MRCIEU/eczema_gwas_fu/blob/master/analysis/cedar/01_cedar_ciseqtl_gemma_r2_p_interval.sh)

**TwinsUK eQTL identification**
```
sh ./analysis/twinsuk/01_twinsuk_ciseqlt_gemma.sh
```
[https://github.com/MRCIEU/eczema_gwas_fu/blob/master/analysis/twinsuk/01_twinsuk_ciseqlt_gemma.sh](https://github.com/MRCIEU/eczema_gwas_fu/blob/master/analysis/twinsuk/01_twinsuk_ciseqlt_gemma.sh)

**TwinsUK eQTL colocalisation with coloc**
```
sh ./analysis/twinsuk/03_twinsuk_r2_p_interval.sh
```
[https://github.com/MRCIEU/eczema_gwas_fu/blob/master/analysis/twinsuk/03_twinsuk_r2_p_interval.sh](https://github.com/MRCIEU/eczema_gwas_fu/blob/master/analysis/twinsuk/03_twinsuk_r2_p_interval.sh)

**eQTLgen eQTL colocalisation with coloc**
```
sh ./colocalization/coloc/06_coloc_analysis_eqtlgen_r2_p_interval.sh
```
[https://github.com/MRCIEU/eczema_gwas_fu/blob/master/colocalization/coloc/06_coloc_analysis_eqtlgen_r2_p_interval.sh](https://github.com/MRCIEU/eczema_gwas_fu/blob/master/colocalization/coloc/06_coloc_analysis_eqtlgen_r2_p_interval.sh)

**Sun et al. (2018) pQTL colocalisation with coloc**
```
sh ./colocalization/coloc/08_coloc_analysis_sun_r2_p_interval.sh
```
[https://github.com/MRCIEU/eczema_gwas_fu/blob/master/colocalization/coloc/08_coloc_analysis_sun_r2_p_interval.sh](https://github.com/MRCIEU/eczema_gwas_fu/blob/master/colocalization/coloc/08_coloc_analysis_sun_r2_p_interval.sh)

**GTEx ver 7 eQTL colocalisation with coloc**
```
sh ./colocalization/coloc/07_coloc_analysis_gtex_r2_p_interval.sh
```
[https://github.com/MRCIEU/eczema_gwas_fu/blob/master/colocalization/coloc/07_coloc_analysis_gtex_r2_p_interval.sh](https://github.com/MRCIEU/eczema_gwas_fu/blob/master/colocalization/coloc/07_coloc_analysis_gtex_r2_p_interval.sh)

**BLUEPRINT eQTL colocalisation with coloc**
```
sh ./colocalization/coloc/10_coloc_analysis_blueprint_r2_p_interval.sh
```
[https://github.com/MRCIEU/eczema_gwas_fu/blob/master/colocalization/coloc/10_coloc_analysis_blueprint_r2_p_interval.sh](https://github.com/MRCIEU/eczema_gwas_fu/blob/master/colocalization/coloc/10_coloc_analysis_blueprint_r2_p_interval.sh)

**Kim-Hellmuth et al. (2017) eQTL colocalisation with coloc**
```
sh ./colocalization/coloc/11_coloc_analysis_kim-hellmuth_r2_p_interval.sh
```
[https://github.com/MRCIEU/eczema_gwas_fu/blob/master/colocalization/coloc/11_coloc_analysis_kim-hellmuth_r2_p_interval.sh](https://github.com/MRCIEU/eczema_gwas_fu/blob/master/colocalization/coloc/11_coloc_analysis_kim-hellmuth_r2_p_interval.sh)

**Plot LocusZoom-like plots for colocalisation results**
```
sh ./colocalization/coloc/09_coloc_analysis_figures.sh
```
[https://github.com/MRCIEU/eczema_gwas_fu/blob/master/colocalization/coloc/09_coloc_analysis_figures.sh](https://github.com/MRCIEU/eczema_gwas_fu/blob/master/colocalization/coloc/09_coloc_analysis_figures.sh)

**CEDAR TWAS analysis**
```
sh ./colocalization/twas/03_twas_analysis_cedar.sh
```
[https://github.com/MRCIEU/eczema_gwas_fu/blob/master/colocalization/twas/03_twas_analysis_cedar.sh](https://github.com/MRCIEU/eczema_gwas_fu/blob/master/colocalization/twas/03_twas_analysis_cedar.sh)

**TwinsUK TWAS analysis**
```
sh ./colocalization/twas/02_twas_analysis_twinsuk_skin.sh
sh ./colocalization/twas/02_twas_analysis_twinsuk_lcl.sh
```
[https://github.com/MRCIEU/eczema_gwas_fu/blob/master/colocalization/twas/02_twas_analysis_twinsuk_skin.sh](https://github.com/MRCIEU/eczema_gwas_fu/blob/master/colocalization/twas/02_twas_analysis_twinsuk_skin.sh)

[https://github.com/MRCIEU/eczema_gwas_fu/blob/master/colocalization/twas/02_twas_analysis_twinsuk_lcl.sh](https://github.com/MRCIEU/eczema_gwas_fu/blob/master/colocalization/twas/02_twas_analysis_twinsuk_lcl.sh)

**GTEx ver 7 TWAS analysis**
```
sh ./colocalization/twas/01_twas_analysis_gtex.sh
```
[https://github.com/MRCIEU/eczema_gwas_fu/blob/master/colocalization/twas/01_twas_analysis_gtex.sh](https://github.com/MRCIEU/eczema_gwas_fu/blob/master/colocalization/twas/01_twas_analysis_gtex.sh)

**PrixFixe network GWAS gene prioritisation**
```
sh ./annotation/networks/02_prixfixe.sh
```
[https://github.com/MRCIEU/eczema_gwas_fu/blob/master/annotation/networks/02_prixfixe.sh](https://github.com/MRCIEU/eczema_gwas_fu/blob/master/annotation/networks/02_prixfixe.sh)

**regfm DHS-sites-based  gene prioritisation**
```
sh ./annotation/regfm/01_regfm_analysis.sh
```
[https://github.com/MRCIEU/eczema_gwas_fu/blob/master/annotation/regfm/01_regfm_analysis.sh](https://github.com/MRCIEU/eczema_gwas_fu/blob/master/annotation/regfm/01_regfm_analysis.sh)



## Individual analyses - variant based
**Variant fine-mapping with FINEMAP**
```
sh ./bayesian_fm/finemap/02_finemap_analysis_1k_euro.sh
```
[https://github.com/MRCIEU/eczema_gwas_fu/blob/master/bayesian_fm/finemap/02_finemap_analysis_1k_euro.sh](https://github.com/MRCIEU/eczema_gwas_fu/blob/master/bayesian_fm/finemap/02_finemap_analysis_1k_euro.sh)

**Variant pruning and fine-mapping with JAM**
```
sh ./bayesian_fm/jam/03_jam_analysis_ukbiobank_euro_30k.sh
```
[https://github.com/MRCIEU/eczema_gwas_fu/blob/master/bayesian_fm/jam/03_jam_analysis_ukbiobank_euro_30k.sh](https://github.com/MRCIEU/eczema_gwas_fu/blob/master/bayesian_fm/jam/03_jam_analysis_ukbiobank_euro_30k.sh)

**Variant fine-mapping with PAINTOR**
```
sh ./bayesian_fm/paintor/02_paintor_analysis_1k_euro.sh
```
[https://github.com/MRCIEU/eczema_gwas_fu/blob/master/bayesian_fm/paintor/02_paintor_analysis_1k_euro.sh](https://github.com/MRCIEU/eczema_gwas_fu/blob/master/bayesian_fm/paintor/02_paintor_analysis_1k_euro.sh)

**Comparison of variant fine-mapping results**
```
sh ./bayesian_fm/integration/01_compare_results.sh
```
[https://github.com/MRCIEU/eczema_gwas_fu/blob/master/bayesian_fm/integration/01_compare_results.sh](https://github.com/MRCIEU/eczema_gwas_fu/blob/master/bayesian_fm/integration/01_compare_results.sh)

**Variant regulatory prediction with KGGSeq**
```
sh ./annotation/KGGSeq/01_KGGSeq_analysis.sh
```
[https://github.com/MRCIEU/eczema_gwas_fu/blob/master/annotation/KGGSeq/01_KGGSeq_analysis.sh](https://github.com/MRCIEU/eczema_gwas_fu/blob/master/annotation/KGGSeq/01_KGGSeq_analysis.sh)

**Variant selection pressure prediction with fitCons**
```
sh ./annotation/fitCons/01_fitCons_annotation.sh
```
[https://github.com/MRCIEU/eczema_gwas_fu/blob/master/annotation/fitCons/01_fitCons_annotation.sh](https://github.com/MRCIEU/eczema_gwas_fu/blob/master/annotation/fitCons/01_fitCons_annotation.sh)


**Individual variant overlap with published highly significant QTLs**
```
sh ./annotation/KGGSeq/01_qtl_overlaps.sh
```
[https://github.com/MRCIEU/eczema_gwas_fu/blob/master/annotation/QTL-overlap/01_qtl_overlaps.sh](https://github.com/MRCIEU/eczema_gwas_fu/blob/master/annotation/QTL-overlap/01_qtl_overlaps.sh)

**Individual variant overlap with promoter-enhancer loops and other functional annotations, such as small RNAs**
```
sh ./annotation/giggle/01_giggle_analysis.sh
```
[https://github.com/MRCIEU/eczema_gwas_fu/blob/master/annotation/giggle/01_giggle_analysis.sh](https://github.com/MRCIEU/eczema_gwas_fu/blob/master/annotation/giggle/01_giggle_analysis.sh)

**SPIDEX: deep learning prediction of splicing sites**
```
sh ./annotation/spidex/01_spidex_analysis.sh
```
[https://github.com/MRCIEU/eczema_gwas_fu/blob/master/annotation/spidex/01_spidex_analysis.sh](https://github.com/MRCIEU/eczema_gwas_fu/blob/master/annotation/spidex/01_spidex_analysis.sh)

## Final integration and locus scoring

**Preparation of standardised input - variant annotation results**
```
sh ./final_integration/02_input_preparation_variant.sh
```
[https://github.com/MRCIEU/eczema_gwas_fu/blob/master/final_integration/02_input_preparation_variant.sh](https://github.com/MRCIEU/eczema_gwas_fu/blob/master/final_integration/02_input_preparation_variant.sh)

**Preparation of standardised input - variant look-up results**
```
sh ./final_integration/01_input_preparation_lookups.sh
```
[https://github.com/MRCIEU/eczema_gwas_fu/blob/master/final_integration/01_input_preparation_lookups.sh](https://github.com/MRCIEU/eczema_gwas_fu/blob/master/final_integration/01_input_preparation_lookups.sh)

**Preparation of standardised input - gene-based results**
```
sh ./final_integration/03_input_preparation_gene.sh
sh ./final_integration/04_input_preparation_gene_secondary.sh
```
[https://github.com/MRCIEU/eczema_gwas_fu/blob/master/final_integration/03_input_preparation_gene.sh](https://github.com/MRCIEU/eczema_gwas_fu/blob/master/final_integration/03_input_preparation_gene.sh)

[https://github.com/MRCIEU/eczema_gwas_fu/blob/master/final_integration/04_input_preparation_gene_secondary.sh](https://github.com/MRCIEU/eczema_gwas_fu/blob/master/final_integration/04_input_preparation_gene_secondary.sh)

**Calculate gene and variant score at each locus and rank. Visualize the results and compare with SMR**
```
sh ./final_integration/05_final_integration.sh
```
[https://github.com/MRCIEU/eczema_gwas_fu/blob/master/final_integration/05_final_integration.sh](https://github.com/MRCIEU/eczema_gwas_fu/blob/master/final_integration/05_final_integration.sh)

## Genomic gene set enrichment

**BEHST: genomic set enrichment analysis enhanced through integration of chromatin long-range interactions**
```
sh ./annotation/behst/01_behst_analysis.sh
```
[https://github.com/MRCIEU/eczema_gwas_fu/blob/master/annotation/behst/01_behst_analysis.sh](https://github.com/MRCIEU/eczema_gwas_fu/blob/master/annotation/behst/01_behst_analysis.sh)

**SNPsea: enrichment analysis to identify cell types, tissues affected by GWAS risk loci**
```
sh ./annotation/snpsea/01_snpsea_analysis.sh
```
[https://github.com/MRCIEU/eczema_gwas_fu/blob/master/annotation/snpsea/01_snpsea_analysis.sh](https://github.com/MRCIEU/eczema_gwas_fu/blob/master/annotation/snpsea/01_snpsea_analysis.sh)
