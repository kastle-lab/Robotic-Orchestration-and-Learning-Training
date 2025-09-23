# Paper Report

**Author:** Shreyas Casturi

## Details

- **Paper Title:** Ontology Development 101: A Guide to Creating Your First Ontology
- **Paper Authors:** Natalya F. Noy and Deborah L. McGuinness

## Report

### Summary

The paper is a guide on how to create an ontology. They explain what an ontology is good for, and then characterize what an ontology actually is (a series of classes `[concepts]`, roles (`[slots]`), role restrictions `[facets]` and instances of classes).

The paper notes there is no single correct way to develop ontologies (another concept that ends up being repeated in all the papers consulted thus far). Some general rules are that developing an ontology is an iterative process, and that you should try to get as close to the real objects you want to model/categorize. 

The general steps to develop an ontology:
1. Determine the domain/scope of ontology -- what will it be used for, what questions should we be able to answer, etc...

2. See if you can reuse existing ontologies

3. Define important terms in the ontology -- what properties, what classes, what roles, etc..

4. Define classes and the hierarchy of classes

5. Define the properties of the classes (the roles, or `slots`). You can break this down into "intrinsic" and "extrinsic" properties, and see what class ties to what role. For example, a Wine class may consist of a date and a color (Date is a Year, color is a string denoting Colors, perhaps a sum-type or enum of some sort).

6. Define facets of the slots (the restrictions), such as how many values a slot can have (cardinality), the type of the value of the slot, etc...

7. Create instances of the classes

You want to pay careful attention to the class hierarchy (ensure that no subclass is a superclass, etc). One thing to note is when to introduce a new class. Generally, introducing a new class happens when there are additional properties that a superclass or other class doesn't have, different restrictions, and/or participation in different relationships. There are some notes about defining the facets, etc... and additional notes about identifiers, delimiters, etc...


### Key Takeaways

1. There is no one way to build an ontology.
2. The best way to judge the efficacy of an ontology is to see what applications can use it, and how productive those applications are.
3. Even though there is no one way to build an ontology, there are heuristic steps you can use that function as a good rule of thumb.

### Questions to Instructor

1. One question I have is that PL theory tends to not favor inheritance, whereas it seems like ontology development is very concerned about class inheritance and even multiple inheritance. Given that ontology development seems so closely linked to strong type systems and other PL concepts that disfavor inheritance, why should ontologies even consider inheritance when there might be other constructs that are more suitable?
