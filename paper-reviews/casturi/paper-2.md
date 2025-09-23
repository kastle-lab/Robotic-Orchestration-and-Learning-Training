# Paper Report

**Author:** Shreyas Casturi

## Details

- **Paper Title:** *A Review of the Semantic Web Field*
- **Paper Authors:** Pascal Hitzler

## Report

### Summary

The author describes the general trend of the Semantic Web field over the past twenty years, starting with the Scientific American article from 2001 (Paper 1's summary covered this) all the way to February 2021.

The Semantic Web, both as an artifact, and as a research field, is hard to define. The author notes that there are two dually related but distinct notions in the field itself: 1: the field is about creating the Semantic Web, defined as a machine-readable Web with intelligent agents (like Paper 1), and a more broader notion that this field is about developing tools to facilitate data transfer between actors, discovery of info, integration into other systems, etc..., aka, a field akin to data science.

The author then reviews three key ideas/technologies that contributed to the Semantic Web in chronological order. First, the author covers ontologies -- knowledge bases that are re-usable and readable by non-human actors, containing both concepts and relationships, formalized in some sort of logic -- which drove the research through the mid 2000s, discussing the emergence of multiple standards for expressing these ontologies and the compatibility between them.

Then, the author discusses the emergence of linked data, which are basically RDF graphs that are linked to one another because these nodes/IDs appear in other graphs. The author notes DBPedia and Wikidata as two major examples. The author notes that the Linked Data graphs were much less complicated and complex than the initial ontology idea, but that the shallow schemas of these graphs made them difficult to reuse/integrate widely: interlinks between data were not enough to integrate disparate datasets.

Then, the author discusses Knowledge Graphs, which became incredibly popular following Google's Knowledge Graph. One major point raises is that the Google Knowledge Graph is proprietary and as a result closed down, contrasting with the Linked Data graphs, and that the Knowledge Graph is more consistent, because it is closed-down and therefore rigidly formalized, whereas Linked Data Graphs have thier own representation schema.

Finally, the author discusses interrelations between The Semantic Web and other CS fields, and notes that one of the biggest future challenges is consolidating the vast amounts of knowledge within the various domains, through the use of applications and data formats.

### Key Takeaways

1. The Semantic Web, though at times difficult to categorize, has made clear advances within the first twenty years of its existence, through the development and systematization of knowledge graphs, linked data, and ontologies.
2. Advances in the infrastructure of the Semantic Web have come from disparate areas of computer science, and have contributed to interrelations and overlap within those originally disparate fields (databases, NLP, AI, knowledge representation).
3. Consolidation of data (in a broad sense) continues to be an open research problem. Being able to consolidate and reuse data will make the Semantic Web much closer to reality.

### Questions to Instructor

1. Was there an expectation that a closed down/proprietary KG would have a negative effect on the research field? Some of the other papers talk about how Semantic Web technologies were meant to facilitate open dissemination of information, yet Google's KG can be queried but the totality of the graph is unknown.
