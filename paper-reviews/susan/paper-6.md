# Paper Report

**Author:** Susan Shrestha

## Details

- **Paper Title:** Knowledge Graphs: Deductive Knowledge
- **Paper Authors:** A. Hogan et al.

## Report

### Summary

Deductive knowledge is about letting a knowledge graph say more than what is explicitly written in it. Given some facts (the graph’s edges/nodes) and some general rules about the world (commonsense or domain rules), we can infer new facts that weren’t stored. Humans do this naturally but machines don’t. As a result we give machines formal instructions (ontologies and entailment rules) that tell them how to draw those conclusions.

### Key Takeaways

1. Deductive rules let the graph imply new facts (e.g., infer a festival’s location) instead of storing every edge by hand.
2. Machine infer via entailment regimes: RDFS/OWL axioms (subclass, subproperty, domain, range), or rule languages (e.g., Datalog) to capture richer if‑then logic.
2. Richer logic yields stronger inferences but can increase complexity; choose the simplest formalism that fits your use case.

### Questions to Instructor