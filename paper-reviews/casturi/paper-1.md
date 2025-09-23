# Paper Report

**Author:** Shreyas Casturi

## Details

- **Paper Title:** *The Semantic Web*
- **Paper Authors:** Tim Berners-Lee, James Hendler, Ora Lassila

## Report

### Summary

The authors posit that the Web (as of May 2001) provides a great deal of information to human actors (people clicking on web pages to produce, acquire, and manipulate data), but it lacks additional information that can better enable computer programs to "make sense" of the data (i.e, to understand the "semantics", or "meaning" of the data).

The authors discuss the "Semantic Web", an addition to/evolution of the current World Wide Web that would have additional information in the web pages, links, and general information networks that would allow computer programs (referred to as "agents") to actually deduce meaning from the web pages in some way. 

The authors note that the key problem is "knowledge representation": how should developers and users encode or represent the key data needed for programs using the Web to operate?

In order to accomplish this, two things must happen: 1. relevant information must be added in a way easily parseable by computer programs, allowing for any sort of structural ordering of information. 2. There must be logical rules/systems the programs can use to make meaning out of the data. These aims are at odds with one another; a system to order information that is inherently flexible complicates and undermines easy logical rules for easy logical inference.

The authors discuss eXtensible Markup Language (XML) and Resource Descriptor Framework (RDF) triples, and Universal Resource Identifiers (URI), which would solve these issues. XML allows users to tag information, but the issue is that a program has to know what the tag means. RDF triples are essentially "subject-verb-object" triples, and so these triples can help programs make assertions about data ("Final Fantasy XIV (Wikipedia)" "is-related-to" "the Final Fantasy franchise articles on Wikipedia"). URIs can help make information unique: a street address is different from an email address, and is different from an address (a speech), and each type of address can be tagged and have additional meaning using RDF + XML.

Thus the authors posit that the Semantic Web will ultimately consist of massive databases of information that "Agents" will trawl over. But each of these databases may have their own rules for inference and understanding of information. How would the Agents know how to make sense of the data for each database? The Agents would need "ontology" files, which basically are files that explain the structure of the data in the database and the rules that govern the usage and production of the data. Using the ontology files, and the standard RDF/XML/URI data, Agents can traverse multiple databases, ingest information, and make inferences/manipulate data.

The transformation of Web data into Semantic Web data will allow agents that ingest diverse information to proliferate and work with one another, using "proofs" of knowledge (one program verifies that you entered correct bank account information, the other program will facilitate a money transfer),  digital signatures (to verify that data or assertions aren't tampered with or forged), etc... But these techniques and ideas build to the final idea, that the Semantic Web is not solely for digital realms. The Semantic Web can catalog and characterize things in the Real World... this anticipates the Internet of Things idea that would come into vogue in the 2010s.

### Key Takeaways

1. The Web is designed for human consumption, not programmatic consumption.
2. In order to facilitate "agents" using the Web, there has to be a way to represent the human knowledge in a way that Agents understand and can make reasoning on top of.
3. The transformation of Web data into Semantic Web data will aid in the production and usage of autonomous agent programs for manipulating and interacting with data.

### Questions to Instructor

1. I want to clarify, the authors were not considering neural-network-based architectures for the agents that they were discussing... the agents here are purely Symbolic AI based (first wave of AI, basically)? So the Agents of the Semantic Web would not require any training to determine inference rules, etc... they'd be able to simply digest those rules via ontology files?

2. Would the Agents be able to read non-English language? For example, what if you were dealing with issues of crime between US and Russian criminal syndicates? In such a case, I could see agents using US criminal databases (in English) and then getting Russian names that were Anglicized and then trying to cross-reference with Cyrillic names from Russian databases. Even with the flexiblity of URI/RDF/XML, I'd think the issue of language would be a problem, because the agent has to read a Russian DB ontology file and somehow have this data interface with primarily English data from the US DB ontology. 

4. Does the Semantic Web idea assume open information sharing in general? What if you have proprietary data, closed APIs, etc...?