# Paper Report

**Author:** Shreyas Casturi

## Details

- **Paper Title:** Knowledge Graphs: Data Graphs
- **Paper Authors:** Hogan et al.

## Report

### Summary

This section of the paper discusses some graph-based models, along with the necessary primitives that are used in graph querying languages.

Specifically, there are:
1. Directed edge-labelled graphs (used in RDF)
2. Heteroegenous graphs, where each node and edge is assigned a type
3. Property graphs
4. Graph dataset (a series of named graphs)
5. Hypergraphs

And ways to store them, as a series of triples, etc...

In order to work with these graphs, we need to develop operations by which we can get information out of the graphs. There are a variety of graph languages for this, such as Sparql, Cypher, etc... As for queries, one example of a necessary query is figuring out the path constructed from a series of nodes.

If you've used Neo4j before, you know what this section is fundamentally about.

### Key Takeaways

1. There is a distinction between the graphs themselves and the tools/features designed to get meaningful information.
2. You can conduct path queries and then use different semantic systems to analyze them, and this may result in cycles.
3. Most queries follow the PL/mathematical intuition that they are composed of smaller queries being put together, just like modular ontologies make up larger ontologies.

### Questions to Instructor

1. Is the graph dataset idea akin to the modular ontology engineering that was discussed in other papers?
