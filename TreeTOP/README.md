# TreeTOP

TreeTOP was Robert McArthur's honours thesis, completed under the supervision of Prof. Gavin Huttley, Dr. Yu Lin, and Dr. Ahad N. Zehmakan.

The honours thesis presents three new algorithms in the field of phylogenetic reconstruction. It should be readable from a non-computational biology background.

It is still under further development and papers will soon be published from this thesis. Stay tuned :)

Original code is at <https://github.com/rmcar17/TreeTOP>, though a cleaner and installable version will release with the papers.

## TripleTree

TripleTree is a new algorithm that is able to reconstruct rooted phylogenetic trees from potentially inconsistent rooted triples. It is fast in solving moderately sized problems with ~100 taxa.

## Spectral Cluster Supertree

Spectral Cluster Supertree will soon be published as a standalone paper. A supertree method is one that merges potentially inconsistent phylogenetic trees into one larger phylogenetic tree. Comparisons against state of the art were not included in the thesis, but I can now reveal that where the current state-of-the-art method, Bad Clade Deletion [1], took ~7000 seconds to solve large problems, spectral cluster supertree can solve the same problems in ~30 seconds.

Robert McArthur was awarded best talk at Phylomania 2023 for this work!

It will soon be published as a package on PyPI. Stay tuned!

## TreeTOP Algorithm

TreeTOP is a new divide-and-conquer algorithm for resolving large rooted phylogenetic trees from DNA sequences of a set of organisms. It combines the previous two algorithms with DCM3 [2] to do this. This will be published in the first half of 2024!

## References

- [1] Fleischauer, Markus, and Sebastian Böcker. "Bad Clade Deletion supertrees: a fast and accurate supertree algorithm." Molecular biology and evolution 34.9 (2017): 2408-2421.
- [2] Roshan, Usman W., et al. "Rec-I-DCM3: a fast algorithmic technique for reconstructing phylogenetic trees." Proceedings. 2004 IEEE Computational Systems Bioinformatics Conference, 2004. CSB 2004.. IEEE, 2004.
