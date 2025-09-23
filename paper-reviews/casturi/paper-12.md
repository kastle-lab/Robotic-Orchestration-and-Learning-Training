# Paper Report

**Author:** Shreyas Casturi

## Details

- **Paper Title:** Knowledge Graphs: Inductive Knowledge
- **Paper Authors:** Hogan et al.

## Report

### Summary

This section of the paper discusses the techniques for enabling induction/rule generalization on knowledge graphs.

Some techniques include unsupervised methods, such as graph analytics (to find clusters in a graph, i.e, sets of nodes that share some generalizing principle), and knowledge graph embeddings that help determine how plausible it is for an edge to be true (this is done via Graph Neural Networks). Additionally, there is symbolic learning, where one looks at the logical formulas of rules + axioms in a graph.

### Key Takeaways

1. It is possible to analyze the semantics of two knowledge graphs rather than the topologies of the graphs (semantically-invariant analytics).
2. Knowledge graph embeddings can be done with either tensor decompositions or translational models.
3. Recursive GNNs deal with fixpoints, whereas ConvGNNs use convolutional layers. 

### Questions to Instructor

1. Which technique or techniques is the most efficient and most accurate?
2. What are the reasons for one set of techniques being more accurate or more efficient than another set? Does this have to do with the structure of the graph, the data inside it, or the technique itself, or is it a mixture of all of these concepts?
