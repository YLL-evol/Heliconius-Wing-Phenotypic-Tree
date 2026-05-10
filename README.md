# Heliconius-Wing-Phenotypic-Tree
Butterfly wing spatial patterns singals builded phenotypic tree compare to genome phylogeny.

## Overview

This project explores phenotypic similarity and convergence in Heliconius butterflies using quantitative wing-pattern data. The notebook constructs a phenotypic distance matrix from wing traits or extracted image features and builds a tree representing morphological similarity among taxa.

The project is motivated by the evolutionary biology of Müllerian mimicry, where unrelated or distantly related butterfly species evolve convergent warning color patterns under predator-mediated selection.

Rather than reconstructing a genomic phylogeny, this analysis investigates whether phenotypic similarity itself forms structured clusters reflecting mimicry, convergence, and adaptive radiation.

Analysis images are from : “Diversité Des Heliconius.” n.d. Accessed April 19, 2026. [https://www.cliniquevetodax.com/Heliconius/](https://www.cliniquevetodax.com/Heliconius/).

## Scientific Question

This project asks:

. Can wing phenotype data reconstruct biologically meaningful similarity relationships among Heliconius butterflies?
. Do convergent mimetic forms cluster together phenotypically?
. How different is a phenotypic tree from a genetic phylogeny?
. Can quantitative morphology reveal adaptive convergence driven by Müllerian mimicry?

## Workflow
1. Data Import

Wing phenotype measurements or image-derived features are loaded into a dataframe.

2. Feature Cleaning
Missing values are removed or imputed.
Non-numeric columns are excluded.
Features are standardized.
3. Distance Matrix Construction

Pairwise Euclidean distances between specimens or taxa are computed using SciPy.

4. Tree Construction

A phenotypic similarity tree is generated using Neighbor Joining or hierarchical clustering methods.

5. Visualization

The resulting tree and distance matrices are visualized to identify phenotypic clustering and convergence.

## Methods

Main Python libraries:

. NumPy
. pandas
. SciPy
. scikit-learn
. BioPython
. matplotlib
. seaborn

Distance metric:

Euclidean distance

Tree method:

. Neighbor Joining (NJ)
. Hierarchical clustering
. Biological Context

Heliconius butterflies are a classic model system for:

. Müllerian mimicry
. adaptive radiation
. convergent evolution
. evo-devo of wing patterning
. genotype–phenotype mapping

Wing coloration is controlled by a relatively small set of major-effect loci, while ecological selection strongly favors convergence between co-mimics.

## Result

Compare to Cicconardi et al. (2023) genomic phylogenetic tree. 

![1. Comparaison to genomic tree.](/Heliconius_pheno_genome_comparaison_tree.PNG)

Compare to introgression events.
![2.](/Heliconius_pheno_introgression_comparaison_tree.PNG)


## References

“Diversité Des Heliconius.” n.d. Accessed April 19, 2026. [https://www.cliniquevetodax.com/Heliconius/](https://www.cliniquevetodax.com/Heliconius/).

Cicconardi, F., Milanetti, E., Pinheiro de Castro, E.C. et al. Evolutionary dynamics of genome size and content during the adaptive radiation of Heliconiini butterflies. Nat Commun 14, 5620 (2023). [https://doi.org/10.1038/s41467-023-41412-5](https://doi.org/10.1038/s41467-023-41412-5)

Hanly, Joseph J., Richard W. R. Wallbank, W. Owen McMillan, and Chris D. Jiggins. 2019. “Conservation and Flexibility in the Gene Regulatory Landscape of Heliconiine Butterfly Wings.” EvoDevo 10 (15). [https://doi.org/10.1186/s13227-019-0127-4.](https://doi.org/10.1186/s13227-019-0127-4)

Hoyal Cuthill, Jennifer F., Nicholas Guttenberg, Sophie Ledger, Robyn Crowther, and Blanca Huertas. 2019. “Deep Learning on Butterfly Phenotypes Tests Evolution’s Oldest Mathematical Model.” Science Advances 5 (8). [https://doi.org/10.1126/sciadv.aaw4967.](https://doi.org/10.1126/sciadv.aaw4967)

Baxter SW, Nadeau NJ, Maroja LS, et al. Genomic hotspots for adaptation: the population genetics of Müllerian mimicry in the Heliconius melpomene clade. PLoS Genet. 2010;6(2):e1000794. Published 2010 Feb 5. [https://doi.org/10.1038/sj.hdy.6800873](https://doi.org/10.1371/journal.pgen.1000794).

Moest, Markus, Steven M. Van Belleghem, Jennifer E. James, Camilo Salazar, Simon H. Martin, Sarah L. Barker, Gilson R. P. Moreira, Claire Mérot, Mathieu Joron, Nicola J. Nadeau, Florian M. Steiner, and Chris D. Jiggins. 2019. “Selective Sweeps on Novel and Introgressed Variation Shape Mimicry Loci in a Butterfly Adaptive Radiation.” PLoS Biology 18 (2). [https://doi.org/10.1371/journal.pbio.3000597](https://doi.org/10.1371/journal.pbio.3000597).

Wu, Grace C., Mathieu Joron, and Chris D. Jiggins. 2010. “Signatures of Selection in Loci Governing Major Colour Patterns in Heliconius Butterflies and Related Species.” BMC Evolutionary Biology 10 (368). [https://doi.org/10.1186/1471-2148-10-368](https://doi.org/10.1186/1471-2148-10-368).
