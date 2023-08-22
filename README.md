# Mustard_Microbiome
scripts for mustard rhizosphere project

## Project Description


### Experimental Question
Does the soil microbial community (bacteria and fungi) influence the flavor chemistry of mustard?

### Methods


## List of files
file explanation, organization

mustard_16S/r_analyses  
01_preprocess.Rmd - cleaning raw ASV table generated with DADA2 (for bacteria)  
02_exploration.Rmd - initial exploration of ASV table, including NMDS plots, mantel tests, PERMANOVAs  
03_correlations.Rmd - loop for checking correlations between individual ASVs and response variable (seed glucosinolate content) *not used in MS or final analyses  
04_RandForestITS.Rmd - random forest model looking for specific ASVs that predict seed glucosinolate content, including ITS data as well (copied from ITS directory)  
04_RandomForest.Rmd - random forest model looking for specific ASVs that predict seed glucosinolate content, 16S data only  
05_DiffAbun.Rmd - differential abundance calculations looking for taxa differentially abundant in "sterile"" versus inoculated soils *not used in MS or final analyses  
06_SoilSlurry.Rmd - analyses of soil slurries and comparison of parent soil to soil slurry  
  
  
mustard_ITS/R.analyses  
01_preprocessing.Rmd - cleaning raw ASV table generated with DADA2 (for fungi)  
02_exploration.Rmd - initial exploration of ASV table, including NMDS plots, mantel tests, PERMANOVAs (very similar to 16S exploration)  
03_FUNGuild.Rmd - preparing and then analyzing data from FUNGuild, an annotation resource for ITS data   
04_RandForestITS.Rmd - - random forest model looking for specific ASVs that predict seed glucosinolate content, including 16S data as well  
  
metagenomics/R_analyses/scripts  
DRAM_annot1.Rmd - Initial version of processing DRAM annotations for testing. Completed on microbe in different script.   

>[!NOTE]
>Large data files including sequence data will be deposited in (...link TBD)