# Paper Report

**Author:** Shreyas Casturi

## Details

- **Paper Title:** Modular Ontology Modeling: A Tutorial
- **Paper Authors:** Cogan Shimizu, Pascal Hitzler, Adila Krisnadhi

## Report

### Summary

This paper discusses an example of Modular Ontology Engineering, using ontology design patterns. The issue with ontologies and schemas is that they require time to maintain as the resulting KG grows in complexity. Trying to overengineer an ontology from the top down results in an ontology that is not reusable/is scoped only to a specific case. 

The key problem is to build ontologies that can be reusable. One way to do that is to build them via modules, and then put the modules together.

The steps towards building the ontology:
1. Define use case
2. Figure out what questions you should be able to ask of the ontology/knowledge base.
3. Determine key notions/patterns from the data and use case (i.e, what ontology design patterns would apply)
4. Create these patterns by invoking the pattern templates, and build modules that way
5. Add axioms for each module
6. Put the modules together.
7. Check that the ontology makes sense after unifying everything.
8. Create OWL files.

The paper notes that OWL doesn't support modularization, so one might need to use namespaces.

### Key Takeaways

1. Generally, building an ontology from the top-down results in overengineering towards a single use case, limiting reusability.
2. Modular ontologies are more reusable, because they've been componentized and each component can be more easily maintained.
3. As with ontology development in general, there is no one-size-fits-all rule, but there are heuristics one can follow.

### Questions to Instructor

1. In one of the other papers on ontology development, they talk about focusing the ontology to the use case. But in this paper, there's an argument that this leads to overengineering to the use case. How should we reconcile these two viewpoints?
2. Is this paper incomplete/ a first draft? Was there supposed to be a description of the Ontology Design Patterns in it? There's also the remark of "I Am the Conclusion."
