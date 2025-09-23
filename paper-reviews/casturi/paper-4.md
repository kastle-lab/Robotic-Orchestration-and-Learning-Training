# Paper Report

**Author:** Shreyas Casturi

## Details

- **Paper Title:** *A Description Logic Primer*
- **Paper Authors:** Markus Krotzsch, Frantisek Simancik, Ian Horrocks 

## Report

### Summary

This paper describes and introduces the notions of Description Logics (DL). DLs are knowledge representation languages that have a formal semantics (i.e, a system by which we can formalize the meaning of DL fragments and ontologies). The power of the DL design has implications on how well reasoning algorithms can perform on data expressed in a DL.

The paper describes ABox, TBox, and RBox axioms: ABox axioms are knowledge about "named individuals", like man(Cogan) (Cogan is a man), or parentOf(Cogan's mom, Cogan) (Cogan's mom is a parent of Cogan). These axioms are about actors and the relationships to which they belong, and the ways they're related to one another.

Notably one has to assert that individuals are different. 

TBox is about describing how concepts are related to one another (all Scientists are examples of Thinkers, i.e, Scientist is a subset of Thinker, for example). 

RBox is about role properties... I'm not clear on this one and will need to ask a question about this.

DLs provide constructors to facilitate the development of new concepts and roles, using Boolean concept constructors (for example, Parents = Father (Union) Mother), role restrictions (someone belonging to the Parent concept is equivalent to someone belonging to the parentOf role, where they are a ParentOf someone else), and nominals (think of these as equivalent to sum-types or enums: Beatles = john | paul | ringo | george), along with some role constructors, such as inverse roles (parentOf and childOf are inverse to one another; one is a parent of a child, one is a child of the parent). These allow us to develop understandings of transitivity and other such relationships (irreflexive, symmetric, asymmetry, disjointness) between individuals, concepts, and roles.

The paper discusses a well known description logic called SROIQ. SROIQ can be used to develop ontologies that are governed by a DL. Every ontology is basically a seto f names, a set of concepts, and a set of roles. SROIQ offers the grammar to capture this, describing what constitutes a role expression, a concept expression, etc... Thus we can formalize ABox, TBox, and RBox axioms.

To ensure that we can reason effectively, we have to make sure the algorithms can terminate which necessitate additional restrictions on the ontologies made via SROIQ. These are the "simplicity" and "regularity" restrictions, which apply to the whole ontology and not just to specific axioms.

The "meaning" of a DL ontology's axioms are through the semantics. Semantics are monotonic -- more axioms leads to more consequences, more knowledge into a DL system results in more results. DLs overall have to deal with incomplete information (but I'm not sure what this means in terms of the open world hypothesis and how certain axioms hold in every state of the world). Need some more info on "interpretations". Overall, the syntax/semantics of the SROIQ constructors looks similar to a programming language's grammar, showing the deep structural interrelationships between programming languages and logics. For each syntactical structure given in the DL, we have a meaning associated with it.

Finally, there are different "fragments" of SROIQ (ALC is another DL that has no RBox axioms and restricts the quantifiers). These fragments are developed to try and make computation and reasoning easier (EL, DLP, DL-Lite, which lign up wigh OWL EL, OWL RL, OWL QL).

DLs and SROIQ in particular are related to OWL Web Ontology Language. OWL is more of an extension to RDF, and RDF's semantics are slightly different from DLs, leading to two different styles of formal semantics: Direct Semantics (DL-based) and RDF-based Semantics. OWL has some other features that DLs don't: naming an ontology, importing one ontology into another, ability to add annotations to arbitrary axioms, etc...


### Key Takeaways

1. Description Logics are used to formalize and develop ontologies and give them a semantics that is readable/usable by machines and humans.
2. Description Logics are fundamentally built from simple syntactic structures, and the composition of these structures allows for ontologies with great expressional depth.
3. OWL and SROIQ have deep interrelationships because they have similar structures.

### Questions to Instructor

1. What are the differences between Concepts and Roles? It seems like they're very close in description/function, so I wanted to better understand this.
2. I was not very clear on why the Open World Hypothesis is needed; I need some clarifications on the role of interpretations in the semantics.
