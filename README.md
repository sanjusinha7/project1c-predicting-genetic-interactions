# Project 1c: Predicting Genetic Interactions

For this project, you will implement and run the featurization and random forest procedure described in [Yu, et al. (Cell Systems, 2016)](http://www.cell.com/cell-systems/abstract/S2405-4712(16)30033-3) on the _S. cerevisiae_ (baker's yeast) data from [Costanzo, et al. (Science, 2010)](http://science.sciencemag.org/content/327/5964/425.long).

### Data

The input data for your algorithm is a matrix of genetic interaction _scores_ for pairs of genes and a hierarchy of gene sets. The genetic interactions are stored in a square [NumPy matrix format](https://docs.scipy.org/doc/numpy/reference/generated/numpy.load.html) with a corresponding file that lists the gene names for the rows/columns. The hierarchy is stored in a tab-separated text file, where each line lists the genes (leaves) in a set (internal node) of the hiearchy.

#### Example data

You can find a small example dataset for your project in [data/examples](https://github.com/cmsc828p-f17/project1c-predicting-genetic-interactions/blob/master/data/examples).

#### Real data

You will need to download real data for your project and process it into the same format as the example data. You will create a _S. cerevisiae_ hierarchy from the [Gene Ontology](http://www.geneontology.org/), and use the genetic interactions data from Costanzo, et al. (Science, 2010). (Costanzo, et al. recently took down their website hosting files from their paper, so you can access a copy I downloaded previously using [this link](https://www.dropbox.com/s/ivsz67jqvkqh0gr/sgadata_costanzo2009_rawdata_101120.txt?dl=0).)
