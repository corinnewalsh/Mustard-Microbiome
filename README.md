# Mustard_Microbiome
scripts for mustard rhizosphere project

## Project Description (ABSTRACT)

>Microorganisms found in the soil may influence the flavor or nutrition of crops, but this hypothesis remains largely untested despite robust evidence for the microbial impact on other plant traits. Our limited understanding of how the soil microbiome may influence food nutrition and flavor chemistry persist because it is challenging to disentangle the impact of soil microbes from other soil and location-specific factors. **Here we measure the independent role of soil microbiomes (bacterial and fungal communities) in determining the flavor chemistry of mustard seed (Brassica juncea).** In a greenhouse study we introduced distinct soil microbial communities to mustard plants growing in an otherwise consistent environment and harvested produced mustard seeds for flavor characterization. We measured the concentration of detectable glucosinolates, a secondary metabolite known to create spicy and bitter flavors. We related rhizosphere microbiome information to seed flavor chemistry information, hypothesizing that differences in rhizosphere microbiomes would result in differences in seed glucosinolate profiles. We found a correlation between the rhizosphere microbiome and the concentration of the main glucosinolate, allyl. We further identified specific taxa and functional genes that may be driving the observed association.

### Experimental Question
#### *Does the soil microbial community (bacteria and fungi) influence the flavor chemistry of mustard?*

### Methods
- Greenhouse experiment with mustard plants (_Brassica juncea_ var Kodiak)  
- Manipulated soil microbes: used five distinct soils collected from different ecosystems to generate distinct microbial community inoculants. Inoculated autoclaved potting soil with live or sterilized soil slurries, or a buffer only control, for a total of 11 different treatment conditions. Each condition had 10 replicate pots, with one mustard plant per pot, for a total of 110 potted mustard plants.   
- Characterized the bacterial (16S rRNA) and fungal (ITS) communities of the roots and rhizospheres of the mustard plants grown in this study via marker gene sequencing, and total community functional potential using shotgun metagenomics.   

## List of files
file explanation, organization

#### mustard_16S/r_analyses
**01_preprocess.Rmd** - cleaning raw ASV table generated with DADA2 (for bacteria)  
**02_exploration.Rmd** - initial exploration of ASV table, including NMDS plots, mantel tests, PERMANOVAs  
**03_correlations.Rmd** - loop for checking correlations between individual ASVs and response variable (seed glucosinolate content) *not used in MS or final analyses  
**04_RandForestITS.Rmd** - random forest model looking for specific ASVs that predict seed glucosinolate content, including ITS data as well (copied from ITS directory)  
**04_RandomForest.Rmd** - random forest model looking for specific ASVs that predict seed glucosinolate content, 16S data only  
**05_DiffAbun.Rmd** - differential abundance calculations looking for taxa differentially abundant in "sterile"" versus inoculated soils *not used in MS or final analyses  
**06_SoilSlurry.Rmd** - analyses of soil slurries and comparison of parent soil to soil slurry  
  
  
#### mustard_ITS/R.analyses
**01_preprocessing.Rmd** - cleaning raw ASV table generated with DADA2 (for fungi)  
**02_exploration.Rmd** - initial exploration of ASV table, including NMDS plots, mantel tests, PERMANOVAs (very similar to 16S exploration)  
**03_FUNGuild.Rmd** - preparing and then analyzing data from FUNGuild, an annotation resource for ITS data   
**04_RandForestITS.Rmd** - random forest model looking for specific ASVs that predict seed glucosinolate content, including 16S data as well  
  
#### metagenomics/R_analyses/scripts
**DRAM_annot1.Rmd** - Initial version of processing DRAM annotations for testing. Completed on microbe in different script.   

>[!NOTE]
>Large data files including sequence data will be deposited in (...link TBD)