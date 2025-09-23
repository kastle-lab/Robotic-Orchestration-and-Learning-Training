# Paper Report

**Author:** Michael McCain

## Details

- **Paper Title:** Knowledge Graphs: Creation and Enrichment
- **Paper Authors:** A. Hogan et al.

## Report

### Summary

This section of the Hogan paper covers the various ways in which useful information can be extracted from multiple sources, such as text, markup, and other structured data. Additionally, it briefly covers the schema and ontology creation process.

### Key Takeaways

1. Using SPARQL queries against an existing KG can be used to filter out unneeded sections of that KG to facilitate the expansion or addition of the target KG.
2. To test ontologies and KGs requires crafting queries that represent the Competency Questions and yield the desired results.
3. `Entity linking` allows entities in text to be associated with nodes in an existing KG. If an entity has aliases, it must be represented in the KG. Additionally, if an entity has multiple candidates for representation in the KG node, the chosen associations can be ranked based on other contextual information within the text.

### Questions to Instructor

1. When validating an ontology or KG, let’s say you don’t get all of the desired data, but some of it. What would be the order of steps for troubleshooting? Would it be best to verify the query matches the competency questions first, then check that the data exists, then verify it has been materialized properly, etc.?

2. How has `Ontology Learning` been applied in practice; do practical examples exist?
