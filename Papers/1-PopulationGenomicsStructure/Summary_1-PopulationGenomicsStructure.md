## Summary discussion on Population genomics, population structure and demography

### Papers discussed:

***Rougemont and Bernatchez 2018***. The demographic history of Atlantic salmon (Salmo salar) across its distribution range reconstructed from approximate Bayesian computations. Evolution: 72-6: 1261–1277.
***Moreno-Mayar et al. 2018***. Early human dispersals within the Americas. Science: 362, eaav2621.

We started the discussion by summarizing the article by Rougemont and Bernatchez. Authors re-analyzed previous global genetic data (> 2,000 samples) of the Atlantic salmon. To understand patterns of population structure and overall demographic history, the authors used three main analytical tools: 1) admixture modeling, 2) geo-genetic assignments, 3) common ancestor graphs and 4) approximate Bayesian computation modelling (ABC). Authors concluded that populations are well differentiated regionally (e. g. North American populations different than European ones) and some minor genetic differences exist among populations within regions. From ABC, the best model of demographic evolution is one that includes a signature of genetic divergence followed by gene flow among populations (i. e. isolation with secondary contact). The group discussed the variation in levels of differentiation among different kinds of SNPs. The data also revealed that most of the migration is happening from populations in North America -with the lowest genetic variation-, to populations in Europe with highest genetic variation. One explanation for this may be that the colonization of North American habitats occurred by the establishment of few founder individuals, which then subsequently mixed with European populations.

Some topics the group discussed include:

*PCA*: A clear representation of the data without much assumptions or any modelling. Clear patterns of differentiation between North America and Europe along PC1, which also had the largest amounts of variation. PCA showed clearly the lower levels of genetic variation in North American populations when compared to those sampled in Europe. PC3 was associated with genetic variation associated with the differentiation of the Iceland population.

*Admixture graphs*: The group thought it was a clear and straight forward representation of the genetic data. The graph depicted differentiated populations such as the “Baltic” or “Iceland” and some admixed ones such as “Barents-White” or “Spain”. The weird pattering/ordering of individuals does not reflect their distribution in the field, but an ad hoc organization based on their admixture coefficient.  

*Common ancestor graphs*: Also known as trees from TreeMix. Results recapitulated those from PCA and admixture plots. The migration bands (in red or yellow) show some level of admixture within and across continents, mostly from Europe to North America.

*Geo-genetic maps*: As PCAs, geogenetic maps, provided a spatial distribution of genetic variation, but unlike PCAs, they present 2D positions of populations (not individuals). Similar to TreeMix, geogenetic maps provide migration bands across populations. In contrast to TreeMix results, most of the migration occurred from North America to Europe.  

The group have a discussion about ABC. The main idea behind this modeling approach is to: 1) Generate models to be tested (isolation without migration, isolation with migration, single panmictic population, etc ..), 2) estimate parameters from the empirical data (e. g. Salmon data) to stablish priors, 3) simulate genealogies under the proposed model, 4) estimate summary statistics (parameters) for the simulated data, 5) compare empirical with simulated data, 6) redo the process from 1 to 6 until you generate enough points (accepted points) to generate a distribution,  7) repeat the process with the next model and repeat the process until you have evaluated all the models. Compare fit of the empirical data to each of the models, rank the models and choose the one with the highest fit. More info [here](https://www.annualreviews.org/doi/10.1146/annurev-ecolsys-110617-062431).

Authors using ABC found a secondary contact as the best demographic model. In brief, populations initially diverged in isolation for approximately one million year and then started mixing. Modeling suggest most of the mixing occurred from North American populations to European ones. The group found a bit problematic making sense of all > 150 models that contained all comparisons. It was also unclear whether the multiple testing of the different models requires a correction technique.

*Genic view of speciation*: A model developed by Chi I Wu to illustrate the gradual progression of genomic differentiation during speciation. Initially, populations only diverge at a very few areas in the genome (often associated with adaptation to different habitats) and then divergence is built around those areas until differentiation is rampant across the whole genome. More info [here](https://onlinelibrary.wiley.com/doi/full/10.1046/j.1420-9101.2001.00335.x).

*Divergence hitchhiking*: A process in which genetic divergence occurs across the genome due to strong divergent selection. Some parts of the “diverging” piece are not under selection nonetheless they hitchhike along with the selective SNP/locus.

*Selective sweep*: A location in the genome with a SNP/locus generally fixed as a result of natural selection. Around the SNP/locus under selection there is usually reduced genetic variation. Because such areas are low in genetic variation, they can be thought of as areas of small population size with higher effects of drift.

*Background selection*: Removal of non-deleterious alleles given their proximity to deleterious ones. It also reduces genetic variation.

The group then enter into a discussion of the Moreno-Maya et al. (2018) article. The group thought this was a hard to read article, yet the application of F-statistics was ingenious and allow for fine-detailed characterization of the migration patterns of humans in North America. F-statistics allows calculation of the magnitude of admixture among populations and those different levels of mixing can be summarized in *qhGraphs*. Here are slinks to get more familiar with F-statistics: [Here](http://www.genetics.org/content/genetics/192/3/1065.full.pdf), [here](https://github.com/DReichLab/AdmixTools/blob/master/README.3PopTest), and [here](https://gaworkshop.readthedocs.io/en/latest/contents/06_f3/f3.html).