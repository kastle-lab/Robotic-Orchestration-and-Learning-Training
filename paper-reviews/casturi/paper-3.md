# Paper Report

**Author:** Shreyas Casturi

## Details

- **Paper Title:** *Industry-Scale Knowledge Graphs: Lessons and Challenges*
- **Paper Authors:** Natasha Noy, Yuqing Gao, Anshu Jain, Anant Narayanan, Alan Patterson, and Jamie Taylor

## Report

### Summary

The article describes, at a broad level, the use of knowledge graphs in the software industry. The article compares five companies (Microsoft, Google, Facebook, eBay, and IBM), and discusses the lessons that have been learned in the construction of these graphs, and what challenges one would face if they needed to construct an "enterprise" level knowledge graph.

First, the article describes the uses of these graphs. Microsoft and Google's graphs support search functionality, whereas Facebook's graph is about the users of the software, describing/cataloguing their likes, dislikes. Ebay's graph is more focused on selling products, so their Product Knowledge Graph is about the relationships between products/objects sold on the market and the people who buy them. IBM's graph is for the AI Watson.

The paper then discusses some of the design decisions that underpin the construction of these graphs. Because each of the companies here have different reasons for using graphs, the construction and decisions regarding the construction of the graphs varies slightly, but there are 2 main principles:

1. Practically all the graphs emphasize capturing complex interrelationships between disparate nodes and trying to see what the implications of those relationships are (Bing and Google for search, eBay for buying things, Facebook for social relationships). 

2. The usefulness of these graphs is in the degree to which they present these three key qualities: Coverage, Correctness, Freshness. Graphs have to cover large swathes of knowledge, be "correct" in the information they have and present, and then have this content be updated in realtime.

Then, each of the graphs presents some challenges. EBay had to deal with providing answers to queries at different timescales (users' queries on the scale of milliseconds, more complex queries took hours), and the implications this had on the architecture and design of the graph, as well as practical considerations regarding the sync up of multiple data stores, among other issues.

Ultimately, there are always issues that are common between all of these KGs: trying to extract knowledge and systematize it, handling it at scale, dealing with different sources of data, dealing with changing data. The fundamental issue of knowledge representation is a difficult one to solve, but its importance to computing systems only grows day by day.

### Key Takeaways

1. All the knowledge graphs presented in the article are strongly typed, that is, the nodes and objects in the graph have specific types and these types govern the construction, behavior, and use of the nodes/objects in the graph. More to the point about the influence of PL in KG theory, there's a point about Google's Knowledge Graph in how "[the graph was] built... from a basic set of low-level structures. It replicated similar structures and reasoning... at different levels of abstraction... Google leveraged the idea that types themselves were instances of types... This meta-level schema also allows validation of data at scale." Let that be some proof that PL theory actually is valuable in industry!
2. The IBM engineers note that "evidence must be primitive to the system", that evidence and presence of knowledge or information is absolutely critical, and that the metadata ABOUT the information is just as important as the information itself when making inferences.
3. One interesting takeaway which lines up with prior articles read on the topic is that a corporation's knowledge graph is not really ONE SPECIFIC graph, but rather an amalgamation of prior graphs (Microsoft has Bing, LinkedIn, the Academic graph, etc).

### Questions to Instructor

1. Is it ever expected that the amount of actual entities will ever dwarf or be much larger than the assertions made about those entities? I wonder if that has implications about the way you capture and format data... as in, it's better to make the parsing and handling of RDF triples (which capture relationships) more efficient on computing systems than structs, which may describe the entities themselves (there are always much less entities than there are relationships; capturing those relationships efficiently is the bottleneck).
2. Is it possible to go one level higher than the knowledge graph to formalize the similarities and differences between the graphs? I wonder if there is some sort of category-theoretic notion to this. 