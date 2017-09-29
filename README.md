# Project 1c: Predicting Genetic Interactions

For this project, you will implement and run the featurization and random forest procedure described in [Yu, et al. (Cell Systems, 2016)](http://www.cell.com/cell-systems/abstract/S2405-4712(16)30033-3) on the _S. cerevisiae_ (baker's yeast) data from [Costanzo, et al. (Science, 2010)](http://science.sciencemag.org/content/327/5964/425.long).

### Data

The input data for your algorithm is a matrix of genetic interaction _scores_ for pairs of genes and a hierarchy of gene sets. The genetic interactions are stored in a square [NumPy matrix format](https://docs.scipy.org/doc/numpy/reference/generated/numpy.load.html) with a corresponding file that lists the gene names for the rows/columns. The hierarchy is stored in a tab-separated text file, where each line lists the genes (leaves) in a set (internal node) of the hiearchy.

#### Example data

You can find a small example dataset for your project in [data/examples](https://github.com/cmsc828p-f17/project1c-predicting-genetic-interactions/blob/master/data/examples).

#### Real data

You will need to download real data for your project and process it into the same format as the example data. You will create a _S. cerevisiae_ hierarchy from the [Gene Ontology](http://www.geneontology.org/).

For genetic interaction data, Yu, et al. used the ~3 million interactions from Costanzo, et al. (Science, 2010). However, because 3 million is probably too many for you to reasonably be able to compute in a short period of time, please use the data from Collins, et al. (Nature, 2007) instead. I've already preprocessed the data, and you can download it from [this link](https://www.dropbox.com/s/git94f7j7avtg62/collins-sc-emap-gis.tsv?dl=0).
