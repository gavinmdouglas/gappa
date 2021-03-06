## Description

Performs [Squash Clustering](http://journals.plos.org/plosone/article?id=10.1371/journal.pone.0056859). The command is a re-implementation of [`guppy squash`](http://matsen.github.io/pplacer/generated_rst/guppy_squash.html), see there for more details.

## Details

The main output of the command is a cluster hierarchy tree that shows which input `jplace` samples are clustered close to each other. Although the tree is written to Newick format, it is not a phylogeny, as its tips represent samples (`jplace` files). The inner node labels are numbered consecutively starting at `n`, with `n ` being the number of samples used as input.

If the `--write-...-tree` options are used, the mass trees representing the samples (tips of the cluster tree) and the mass trees of the inner nodes (average masses of the corresponding tips) are written for visualization. Their numbering is `0` to `n-1` for the tips (samples), and `n` to `2n-2` for the inner nodes (cluster averages). These trees can help to explore how and why the samples were clustered during the algorithm.

## Citation

When using this method, please do not forget to cite

> Matsen FA, Evans SN (2013),
> **"Edge Principal Components and Squash Clustering: Using the Special Structure of Phylogenetic Placement Data for Sample Comparison."**,
> *PLOS ONE 8(3): e56859*, doi:[10.1371/journal.pone.0056859](http://journals.plos.org/plosone/article?id=10.1371/journal.pone.0056859)
