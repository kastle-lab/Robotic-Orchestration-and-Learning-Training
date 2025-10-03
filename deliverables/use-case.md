# Use Case

## Narrative

Domains that rely heavily on robotics have shown an increasing interest in autonomous systems that are collaborative, intelligent, and capable of reasoning [1, 2]. In pursuit of these interests, a standard method for increasing autonomy among robots [2] and enabling collaboration is the use of knowledge representation in the form of ontologies [3] and knowledge graphs [2, 4]. Due to the relatively recent focus on achieving these ambitious and complex autonomous systems, there are many competing approaches, especially in the context of task planning [1, 2, 4, 5, 6, 7]. However, many of these approaches vary in terms of ontology design or methodology, but do use OWL as the primary language for semantic representation [2].

Considering these aspects for the current ontological representations of complex autonomous systems, we want to engineer an ontology that could enable these multi-agent systems [8] to be governed and commanded by an AI Orchestrator capable of understanding its environment, decomposing goals into atomic subtasks, and assigning agents to complete these tasks based on their capabilities. This ontology would be designed using state-of-the-art best practices to ensure modularity through the use of ontological design patterns (ODPs) and reusability [9].

## Competency Questions

- What set of `agents` are required to complete `primary goal` _y_?<br>
- Which `agent` can perform `task` _z_?<br>
- What `agents` are required to complete `task` _x_? <br>

Bridges Datasets: [Droid](https://droid-dataset.github.io/), [LaViA](https://gatech.app.box.com/s/5onzr6sj99jpcsee1sgo7gztpqui4z2p),
[RH20T-P](https://sites.google.com/view/rh20t-primitive/main)

---

- What is the sequence(`task list`) of `tasks` required to complete `primary goal` _g_?<br>
- What are the `dependent tasks` for `task` _z_? <br>
- What `goals` can be achieved from `task` _X_?<br>
- Which `tasks` share common `dependent tasks` across different `goals`?

Bridges Datasets: [MOAD](https://www.robot-manipulation.org/nist-moad),
[ALFRED](https://askforalfred.com/), [EpicKitchens](https://epic-kitchens.github.io/2025), [RH20T-P](https://sites.google.com/view/rh20t-primitive/main)

---

- What `tasks` are decomposable? <br>
- What `tasks` consist of at least _X_ `tasks`? <br>
- What `tasks` are the atomic level `tasks`? <br>
- Which `task(s)` require collaboration between multiple `agents`? <br>

Bridges Datasets: [RH20T-P](https://sites.google.com/view/rh20t-primitive/main), [DROID](https://droid-dataset.github.io/)

---

- Which `agent` has `priority` to do `task` _z_ if `agent` _A_ and `agent` _B_ are on a collision?<br>
- What were the `states` of the `agent` following a failed `task`? <br>
- What is an alternative `path` from `task` _x_ to `task` _y_? <br>
- What should be the estimated `time` to complete `task` _x_ by `agent` _A_?<br>

Bridges Datasets: [DROID](https://droid-dataset.github.io/), [Workcell manufacturing operations](https://catalog.data.gov/dataset/process-and-robot-data-from-a-two-robot-workcell-representative-performing-representative-), [Robot-World Hand-Eye(s)](https://catalog.data.gov/dataset/data-from-solving-the-robot-world-hand-eyes-calibration-problem-with-iterative-methods-02035)

---

- What are the `classifications`/`categories` that of a set of `objects`? <br>

Bridges Datasets: [Scanned Objects by Google](https://research.google/blog/scanned-objects-by-google-research-a-dataset-of-3d-scanned-common-household-items/)
, [Princeton Model Net](https://modelnet.cs.princeton.edu/#)

---

- What `objects` are required to complete `task` _x_? <br>
- What are the `task(s)` that can be achieved by the presence of `object` _o_? <br>
- What `objects` are required for `goal` _g_? <br>

Bridges Datasets: [BridgeData V2](https://rail-berkeley.github.io/bridgedata/), [EpicKitchens](https://epic-kitchens.github.io/2025), [RH20T-P](https://sites.google.com/view/rh20t-primitive/main), [ALFRED](https://askforalfred.com/)

---

## Potential Datasets

1. [LaViA](https://gatech.app.box.com/s/5onzr6sj99jpcsee1sgo7gztpqui4z2p)
2. [NIST-Manufacturing Objects for Assembly Database (MOAD) ATB dataset](https://www.robot-manipulation.org/nist-moad)
3. [DROID](https://droid-dataset.github.io/)
4. [Process and robot data from a two robot workcell representative performing representative manufacturing operations](https://catalog.data.gov/dataset/process-and-robot-data-from-a-two-robot-workcell-representative-performing-representative-)
5. [Data from: Solving the Robot-World Hand-Eye(s) Calibration Problem with Iterative Methods](https://catalog.data.gov/dataset/data-from-solving-the-robot-world-hand-eyes-calibration-problem-with-iterative-methods-02035)
6. [EpicKitchens](https://epic-kitchens.github.io/2025)
7. [ALFRED](https://askforalfred.com/)
8. [RH20T-P: A Primitive-Level Robotic Dataset Towards Composable Generalization Agents](https://sites.google.com/view/rh20t-primitive/main)
9. [Autonomously Constructing Hierarchical Task Networks for Planning and Human-Robot Collaboration](https://scazlab.yale.edu/sites/default/files/files/hayes_icra16.pdf)
10. [BridgeData V2](https://rail-berkeley.github.io/bridgedata/)

## References

[1] A. Olivares-Alarcos, S. Foix, S. Borgo, and None Guillem Alenyà, “OCRA – An ontology for collaborative robotics and adaptation,” Computers in Industry, vol. 138, pp. 103627–103627, Feb. 2022, doi: https://doi.org/10.1016/j.compind.2022.103627

[2] E. Aguado, V. Gomez, M. Hernando, C. Rossi, and R. Sanz, “A survey of ontology-enabled processes for dependable robot autonomy,” Frontiers in Robotics and AI, vol. 11, Jul. 2024, doi: https://doi.org/10.3389/frobt.2024.1377897

[3] A. Ricci, M. Piunti, and M. Viroli. Environment programming in multi-agent systems: an artifact-based perspective. Autonomous Agents and Multi-Agent Systems, 23:158–192, 2011.

[4] H. Li et al., “IEEE Standard for Autonomous Robotics (AuR) Ontology,” Sep. 2021, doi: https://doi.org/10.1109/ieeestd.2022.9774339.

[5] X. Sun, Y. Zhang, and J. M. Chen, “RTPO: A Domain Knowledge Base for Robot Task Planning,” vol. 8, no. 10, pp. 1105–1105, Oct. 2019, doi: https://doi.org/10.3390/electronics8101105.

[6] C. Z. Sprenger, J. Antonio, and N. U. Baier, “ORPP—An Ontology for Skill-Based Robotic Process Planning in Agile Manufacturing,” Electronics, vol. 13, no. 18, pp. 3666–3666, Sep. 2024, doi: https://doi.org/10.3390/electronics13183666.

[7] L. Kinder and T. Käfer, “Static and Adaptive Planning with WoT TD by Generating Python Objects as Intermediary Representations Using Large Language Models,” Lecture notes in computer science, pp. 256–273, Jan. 2025, doi: https://doi.org/10.1007/978-3-031-78955-7_21

[8] H. Du, S. Thudumu, R. Vasa, and K. Mouzakis, “A Survey on Context-Aware Multi-Agent Systems: Techniques, Challenges and Future Directions,” arXiv.org, 2024. Available: https://arxiv.org/abs/2402.01968v2. [Accessed: Feb. 26, 2025]

[9] A. Hogan et al., “Knowledge Graphs,” ACM Computing Surveys, vol. 54, no. 4, pp. 1–37, May 2022, doi: https://doi.org/10.1145/3447772
