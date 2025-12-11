# Use Case

## Narrative

Domains that rely heavily on robotics have shown an increasing interest in autonomous systems that are collaborative, intelligent, and capable of reasoning [1, 2, 3]. In pursuit of these interests, a standard method for increasing autonomy among robots [2] and enabling collaboration is the use of knowledge representation in the form of ontologies [4] and knowledge graphs (KG) [2, 3, 5]. Due to the relatively recent focus on achieving these ambitious and complex autonomous systems, there are many competing approaches, especially in the context of task planning [1, 2, 5, 6, 7, 8]. However, these approaches vary in terms of ontology design or methodology, but do use the World Wide Web Consortium (W3C) consortium’s Web Ontology Language (OWL) [9] as the primary logic-based language for semantic representation. Unfortunately, as highlighted in [2], many of these ontologies lack reusability and do not meet the need for the confluence of existing ontologies.

Considering these aspects for the current ontological representations of complex autonomous systems, we want to engineer an ontology that could enable these multi-agent systems (MAS) [3] to be governed and commanded by an AI Orchestrator capable of the following: understanding its environment, decomposing goals into atomic subtasks, agent assignment based on capabilities, and status verification. More importantly, it would be designed to be general enough to support reusability and allow for adaptation to the domain of need. This ontology would be designed using state-of-the-art (SOTA) best practices to ensure modularity and reusability [10, 11] through the use of ontological design patterns (ODPs) [12]. This would fill two needs. The first would be to provide an ontology that allows for more complex autonomous MAS. The second is the demand for a reusable ontology that facilitates the merging of existing ontologies across domains that utilize these MAS.

## Competency Questions

**Robot Capability Requirements**: This set of CQs focuses primarily on the identification of robots with respect to their specialization or capabilities for/towards specific tasks or goals.

- What set of `agents` are required to complete `primary goal` _y_?<br>
- Which `agent` can perform `task` _z_?<br>
- What `agents` are required to complete `task` _x_? <br>

Bridges Datasets: [Droid](https://droid-dataset.github.io/), [LaViA](https://gatech.app.box.com/s/5onzr6sj99jpcsee1sgo7gztpqui4z2p),
[RH20T-P](https://sites.google.com/view/rh20t-primitive/main)

---

**Task Analysis and Decomposition**: This set of CQs focuses mainly on task-specific intricacies like dependencies, hierarchies, accounting for both part-of decompositions, sequence/order of tasks to be done, all towards another task or a specific goal.

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

**Environment and Execution in Orchestration**: This set of questions focuses on collaboration and orchestration priorities between different robots for similar tasks, within the context of the environment.

- Which `agent` has `priority` to do `task` _z_ if `agent` _A_ and `agent` _B_ are on a collision?<br>
- What were the `states` of the `agent` following a failed `task`? <br>
- What is an alternative `path` from `task` _x_ to `task` _y_? <br>
- What should be the estimated `time` to complete `task` _x_ by `agent` _A_?<br>

Bridges Datasets: [DROID](https://droid-dataset.github.io/), [Workcell manufacturing operations](https://catalog.data.gov/dataset/process-and-robot-data-from-a-two-robot-workcell-representative-performing-representative-), [Robot-World Hand-Eye(s)](https://catalog.data.gov/dataset/data-from-solving-the-robot-world-hand-eyes-calibration-problem-with-iterative-methods-02035)

---

**Object/Environment Analysis**: This set of questions focuses on datasets of objects and environmental factors that would be relevant to the task at hand.

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

[1] A. Olivares-Alarcos, S. Foix, S. Borgo, N. G. Alenyà, Ocra – an ontology for collaborative robotics and adaptation, Computers in Industry 138 (2022) 103627–103627. doi:10.1016/j.compind.2022.103627.

[2] E. Aguado, V. Gomez, M. Hernando, C. Rossi, R. Sanz, A survey of ontology-enabled processes for dependable robot autonomy, Frontiers in Robotics and AI 11 (2024). doi:10.3389/frobt.2024.1377897.

[3] H. Du, S. Thudumu, R. Vasa, K. Mouzakis, A survey on context-aware multi-agent systems: Techniques, challenges and future directions, 2024. URL: https://arxiv.org/abs/2402.01968v2.

[4] A. Ricci, M. Piunti, M. Viroli, Environment programming in multi-agent systems: an artifact-based perspective, Autonomous Agents and Multi-Agent Systems 23 (2010) 158–192. doi:10.1007/s10458-010-9140-7.

[5] H. Li, P. Goncalves, V. Ragavan, A. Olivares-Alarcos, E. M. Barreto, D. Beβler, J. Bermejo, S. Borgo, A. Chibani, J. Carbonera, M. Diab, S. Fiorini, A. Gyrard, M. Habib, A. Khamis, K. Moulouel, H. Nakawala, B. Nguyen, C. Nowak, J. Olszewska, E. Pignaton, E. Prestes, J. Quintas, S. Redfield, R. Sanz, C. Schlenoff, E. Tosello, Ieee standard for autonomous robotics (aur) ontology (2021). URL: https://ieeexplore.ieee.org/document/9774339?utm_source=chatgpt.com. doi:10.1109/ieeestd. 2022.9774339.

[6] X. Sun, Y. Zhang, J. M. Chen, Rtpo: A domain knowledge base for robot task planning 8 (2019) 1105–1105. doi:10.3390/electronics8101105.

[7] C. Z. Sprenger, J. Antonio, N. U. Baier, Orpp—an ontology for skill-based robotic process planning in agile manufacturing, Electronics 13 (2024) 3666–3666. URL: https://www.mdpi.com/2079-9292/13/18/3666. doi:10.3390/electronics13183666.

[8] L. Kinder, T. Käfer, Static and adaptive planning with wot td by generating python objects as intermediary representations using large language models, Lecture notes in computer science (2025) 256–273. doi:10.1007/978-3-031-78955-7_21.

[9] W. W. W. C. (W3C), Owl 2 web ontology language primer (second edition), URL: https://www.w3.org/TR/2012/REC-owl2-primer-20121211/.

[10] C. Shimizu, Q. Hirt, P. Hitzler, Modl: A modular ontology design library, 2019. URL: https://arxiv.org/abs/1904.05405.

[11] C. Shimizu, K. Hammar, P. Hitzler, Modular ontology modeling, Semantic Web (2022) 1–31. doi:https://doi.org/10.3233/sw-222886.

[12] A. Hogan, E. Blomqvist, M. Cochez, C. D’amato, G. D. Melo, C. Gutierrez, S. Kirrane, J. E. L. Gayo, R. Navigli, S. Neumaier, A.-C. N. Ngomo, A. Polleres, S. M. Rashid, A. Rula, L. Schmelzeisen, J. Sequeda, S. Staab, A. Zimmermann, Knowledge graphs, ACM Computing Surveys 54 (2022) 1–37. doi:10.1145/3447772.
