# Paper Report

**Author:** Chris Davis Jaldi

## Details

- **Paper Title:** Knowledge Graphs: Data Graphs
- **Paper Authors:** A. Hogan et al.

## Report

### Summary

This section introduces and explores many different foundational data graphs, wrt to various graph models, and their respective querying and navigation strategies.
Interesting models include:

- Directed Edge-Labelled Graphs
- Heterogeneous Graphs
- Property Graphs
- Hypergraphs

### Key Takeaways

1. Some models (Directed Edge-Labelled Graphs) offer superior flexibility for evolving, schema-light data compared to relational databases than others.
2. Availability of different navigational and querying approaches which can be optimal for specific task sets.
3. Multiple strategies and graph models exist and can often be transformed between one another allowing to choose implementations based on performance and application needs.

### Questions to Instructor

1. Looking at all of these models avaialble, isnt the class or even more broadly (the KASTLE) standard, just a complete/partial adoption of all for the best of all worlds?
2. How do some of these querying methods through some navigational graph patterns handle infinite paths, espcially with cyclic graphs? What are design considerations for query bounds then?
3. is SPARQL the only querying language which preserves the complete KG semantics and not work on regex like searches?
