# CEGARBox: An Efficient Theorem Prover for the 15 Normal Modal Cube Logics

CEGARBox [1] is a state-of-the-art modal logic theorem prover. In this project I worked under Prof. Rajeev Goré to extend this theorem prover.

Modal logic is an extension of classical logic that introduces two new operators - box and diamond.
box(p) means "p is true in all successor worlds", and diamond(q) means "there exists a successor world where q is true".

There are different axioms that can be added, such as reflexivity, symmetry, transitivity, seriality and euclideanness which restricts the successor relations.
For example, under reflexivity every world is a sucessor of itself. Under symmetry if "a" is a successor of "b" then "b" is a successor of "a".

The different combinations of these axioms give the 15 normal modal cube logics.

There is also multi-modal logic, where each of the successor relations are labelled. For example, box(1,p) would mean "in all successors of type 1, p is true", and diamond(2,q) would mean "there exists a successor of type 2 such that q is true".

In this project, I extended the theorem prover to handle all 15 normal modal cube logics, as well as multi-modal logic. This is discussed in the research report in this folder (~30 pages of content).

Over the summer, I continue my work under Goré. I extended the theorem prover to handle tense logic. Tense logic is a variant of modal logic with operators blackbox, blackdiamond, whitebox, whitediamond. The definitions are similar, though whitebox and whitediamond are used to refer to worlds in the future, and blackbox and blackdiamond are used to refer to worlds in the past.

For example, (whitediamond(T) & whitebox(blackbox(p))) => p. That is, whitediamond create a future world, and in the future world, all past worlds have p as true. Therefore p is true.

Further extensions such as to linear temporal logic are underway prior to publication. The most recent version of the code can be found at <https://github.com/cormackikkert/CEGARBoxCPP/>

## References

- [1] Goré, Rajeev, and Cormac Kikkert. "CEGAR-tableaux: improved modal satisfiability via modal clause-learning and SAT." Automated Reasoning with Analytic Tableaux and Related Methods: 30th International Conference, TABLEAUX 2021, Birmingham, UK, September 6–9, 2021, Proceedings 30. Springer International Publishing, 2021.
