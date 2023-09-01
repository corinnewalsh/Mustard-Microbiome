# Mustard_Microbiome
scripts for mustard rhizosphere project

## Project Description (ABSTRACT)

>Microorganisms found in the soil may influence the flavor or nutrition of crops, but this hypothesis remains largely untested despite robust evidence for the microbial impact on other plant traits. Our limited understanding of how the soil microbiome may influence food nutrition and flavor chemistry persist because it is challenging to disentangle the impact of soil microbes from other soil and location-specific factors. **Here we measure the independent role of soil microbiomes (bacterial and fungal communities) in determining the flavor chemistry of mustard seed (Brassica juncea).** In a greenhouse study we introduced distinct soil microbial communities to mustard plants growing in an otherwise consistent environment and harvested produced mustard seeds for flavor characterization. We measured the concentration of detectable glucosinolates, a secondary metabolite known to create spicy and bitter flavors. We related rhizosphere microbiome information to seed flavor chemistry information, hypothesizing that differences in rhizosphere microbiomes would result in differences in seed glucosinolate profiles. We found a correlation between the rhizosphere microbiome and the concentration of the main glucosinolate, allyl. We further identified specific taxa and functional genes that may be driving the observed association.

### Experimental Question
#### *Does the soil microbial community (bacteria and fungi) influence the flavor chemistry of mustard?*

### Methods
- Greenhouse experiment with mustard plants (_Brassica juncea_ var Kodiak)  
- Manipulated soil microbes: used five distinct soils collected from different ecosystems across CO to generate distinct microbial community liquid inoculants. Inoculated autoclaved potting soil with live or sterilized soil slurries, or a buffer only control, for a total of 11 different treatment conditions. Each condition had 10 replicate pots, with one mustard plant per pot, for a total of 110 potted mustard plants.   
- Characterized the bacterial (16S rRNA) and fungal (ITS) communities of the roots and rhizospheres of the mustard plants grown in this study via marker gene sequencing, and total community functional potential using shotgun metagenomics.  
- Characterized the chemical profile of mustard seeds produced, focusing on the major flavor chemical of brassica: glucosinolates. Glucosinolate testing performed at UC Davis in the lab of Dan Kliebenstein. 

## List of files
file explanation, organization

#### mustard_16S/r_analyses
**01_preprocess.c.Rmd** - cleaning raw ASV table generated with DADA2 (for bacteria)  
**02_exploration.c.Rmd** - initial exploration of ASV table, including NMDS plots, mantel tests, PERMANOVAs  
**03_mantels.c.Rmd** - mantel tests looking at associations between rhizosphere community and seed composition, etc  
**03.5_RDA.c.Rmd** - distanced based RDA, constraining ordination to seed chemistry variables  
**04_RandForestALL.c.Rmd** - random forest model looking for specific ASVs that predict seed glucosinolate content, 16S and ITS data


#### mustard_ITS/R.analyses
**01_preprocessing.c.Rmd** - cleaning raw ASV table generated with DADA2 (for fungi)  
**02_exploration.c.Rmd** - initial exploration of ASV table, including NMDS plots, mantel tests, PERMANOVAs (very similar to 16S exploration)  
**03_FUNGuild.c.Rmd** - preparing and then analyzing data from FUNGuild, an annotation resource for ITS data   

#### mustard_chem/code
**chem_analysis.c.Rmd** - cleaning plant metadata and plant seed chemistry data, initial exploration into associations between plant phenotypic data

#### mustard metagenomic scripts still in progress, not public

>[!NOTE]
>Large data files including sequence data will be deposited in (...link TBD)
