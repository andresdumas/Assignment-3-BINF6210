# Assignment-3-BINF6210

############################################################################-
##-----------------------------INTRODUCTION----------------------------------
############################################################################-

#The genus Rana has more than 100 species ranging across Europe, Asia, North America and South America. This spatial distribution and richness in species make them a good group to explore evolutionary processes and test different biologic hypothesis (Yuan et al., 2016). On the other hand, the morphology of frogs in Rana genus is generally conserved, specially in the Erasian species, making them difficult to be identified. Recently molecular analysis have helped in the identification of new species and more cryptic species are suggested to occur mainly in America (Zhao et al., 2017). 
#There are four main classes of molecular markers for species identification and systematic, nuclear rRNAs such as 18S and 28S, nuclear spacers such as ITS1 and ITS2, mt protein-coding genes such as COI and cytB and mt rRNAs such as 12S and 16S (Chan et al., 2021). Being the COI gene one of the most broadly used for species identification. The aim of this study is to compare the efficiency of the genes COI and CYTB for species identification in the Rana genus based on a clustering algorithm.

############################################################################-
##-----------------------------DISCUSSION------------------------------------
############################################################################-
#Based on the results obtained we can infer that the COI gene would be a good candidate for clustering identification in the Rana genus. We obtained a better clustering pattern in the silhouette plot for COI gene as values are near one. In contrast, in the silhouette plot for CYTB we obtained an average of 0.70 and a value near zero in cluster seven and a negative value in cluster ten indicating a bad clustering and similar boundaries between clusters (Figure 2) (Scikit-learn Developers, 2021). In the case of dendrograms, we observed acceptable distances of the branches for both genes but a better differentiation of clusters for COI gene (Figure 3 & 4).
#High quality sequences in general were used, maintaining similar sequence length for each gene with very few missing data to be able to generate reproducible data. In this case the default parameters for alignment of both sequences were used and the same model of evolution for clustering was used (Figure 1) In future studies it would be recommended to test different parameter to evaluate how they influence the clustering pattern. Despite many studies use DNA for clustering and even phylogeny it would be recommended to translate the sequences to aminoacids and run the whole analysis to compare results.

############################################################################-
##-----------------------------SCRIPTS----------------------------------
############################################################################-

#Script_Assignment_2 runs a complete analysis on COI and CYTB sequences from the Rana genus. The script is divided into: libraries, preliminary data search, data fetching (using Entrez_Funcions.R), sequence alignment, sequence clustering and visualizations. 
#In the visualizations section, it generates 2 merged histograms of sequence lenghts, 2 merged silhouette plots and 2 separate dendrograms which are generated locally (they can be found on the working directory).
