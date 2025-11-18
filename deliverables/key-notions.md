# Key Notions

- **Capability**
  - <u><b>Rationale</b></u>: Specifications to differentiate and define what actions an agent can perform (E.g., Grab, Push, Pull, Lift, Travel, Etc.).
  - <u>**Connected Pattern**</u>: [role-dependent-name](https://github.com/kastle-lab/modular-ontology-design-library/tree/master/modl/role-dependent-name),
  - <u>**Source Dataset(s)**</u>: [Droid](https://droid-dataset.github.io/), [LaViA (no longer accessible)](https://gatech.app.box.com/s/5onzr6sj99jpcsee1sgo7gztpqui4z2p), [RH20T-Ps](https://sites.google.com/view/rh20t-primitive/main)

---

- **Agent**
  - <u>**Rationale**</u>: A default representation of an entity (robotic) capable of interacting with its environment.
  - <u>**Connected Pattern**</u>: [agent-role](https://github.com/kastle-lab/modular-ontology-design-library/blob/master/modl/agent-role/agent-role-pattern.pdf), [OntoPret]()
  - <u>**Source Dataset(s)**</u>: [RH20T-Ps](https://sites.google.com/view/rh20t-primitive/main)

---

- **Provenance**
  - <u>**Rationale**</u>: To identify which multi-agent (MAS) system a robotic agent originates from. Captures the origin, role, and contextual metadata associated with architype and goal.
  - <u>**Connected Pattern**</u>: [provenance](https://github.com/kastle-lab/modular-ontology-design-library/blob/master/modl/provenance/provenance-pattern.pdf)
  - <u>**Source Dataset(s)**</u>: [Droid](https://droid-dataset.github.io/), [RH20T-P](https://sites.google.com/view/rh20t-primitive/main)

---

- **Archetype**
  - <u>**Rationale**</u>: Representing the thematic capabilities of a robotic agent (E.g., Explorer, Hauler, Designer, Painter, etc.).
  - <u>**Connected Pattern**</u>: [participant-role](https://github.com/kastle-lab/modular-ontology-design-library/blob/master/modl/participant-role/participant-role-pattern.pdf), [OntoPret]()
  - <u>**Source Dataset(s)**</u>: TBD

---

- **State**
  - <u>**Rationale**</u>: Representing the state, state transitions, and state space of an agent. Useful for predicting and correcting actions, as well as identifying deviations.
  - <u>**Connected Pattern**</u>: [state-transition](https://github.com/kastle-lab/modular-ontology-design-library/blob/master/modl/state-transition/state-transition-pattern.pdf)
  - <u>**Source Dataset(s)**</u>: [Droid](https://droid-dataset.github.io/), [LaViA](https://gatech.app.box.com/s/5onzr6sj99jpcsee1sgo7gztpqui4z2p),
    [RH20T-P](https://sites.google.com/view/rh20t-primitive/main)

---

- **Event**
  - <u><b>Rationale:</b></u> Capturing the specific things that just happened at a certain point of time, like when robot gripper confirms it has successfully picked up its target. The action is the trigger that causes the robot's State to change from executing to idle.
  - <u><b>Connected Pattern:</u></b> [event](https://github.com/kastle-lab/modular-ontology-design-library/blob/master/modl/event/event-pattern.pdf), [description-situation](https://github.com/kastle-lab/modular-ontology-design-library/blob/master/modl/description-situation/description-situation-pattern.pdf),
    [causal-event](https://github.com/kastle-lab/modular-ontology-design-library/blob/master/modl/causal-event/causal-event-pattern.pdf), [recurrent-event](https://github.com/kastle-lab/modular-ontology-design-library/blob/master/modl/recurrent-event/recurrent-event-pattern.pdf), [reporting-event](https://github.com/kastle-lab/modular-ontology-design-library/blob/master/modl/reporting-event/reporting-event-pattern.pdf)
  - <u><b>Source Dataset(s):</b></u> [Droid](https://droid-dataset.github.io/), [RH20T-P](https://sites.google.com/view/rh20t-primitive/main), [BridgeData V2](https://rail-berkeley.github.io/bridgedata/)

---

- **Environment**
  - <u><b>Rationale:</b></u> Provide shared situational awareness for all Agents telling the orchestrator where the Agents can go, where Objects are, and what areas are restricted which is essential for planning safe and successful Tasks.
  - <u><b>Connected Pattern:</u></b> [observation](https://github.com/kastle-lab/modular-ontology-design-library/blob/master/modl/observation/observation-pattern.pdf), [part-whole](https://github.com/kastle-lab/modular-ontology-design-library/blob/master/modl/part-whole/part-whole-pattern.pdf)
  - <u><b>Source Dataset(s):</b></u> [Scanned Objects by Google](https://research.google/blog/scanned-objects-by-google-research-a-dataset-of-3d-scanned-common-household-items/)
    , [Princeton Model Net](https://modelnet.cs.princeton.edu/#), [NIST-Manufacturing Objects for Assembly Database (MOAD) ATB dataset](https://www.robot-manipulation.org/nist-moad), [EpicKitchens](https://epic-kitchens.github.io/2025), [DROID](https://droid-dataset.github.io/)

---

- **Temporal**
  - <u><b>Rationale:</b></u> It's a **when**(timestamp) for recording Events and provides the **how long**(duration) for scheduling Tasks, so you have perfect timeline of everything that happened.
  - <u><b>Connected Pattern:</u></b> [temporal-extent](https://github.com/kastle-lab/modular-ontology-design-library/blob/master/modl/temporal-extent/temporal-extent-pattern.pdf)
  - <u><b>Source Dataset(s):</b></u> TBD

---

- **Namestub**
  - <u><b>Rationale:</b></u> : It's basically a **nametag** pattern. It's a simple, reusable way to give anything (like an Agent, Task, or Object) a human-readable name.
  - <u><b>Connected Pattern:</u></b> [name-stub](https://github.com/kastle-lab/modular-ontology-design-library/blob/master/modl/name-stub/name-stub-pattern.pdf)
  - <u><b>Source Dataset(s):</b></u> TBD

---

- **Task**

  - <u>**Rationale**</u>: Represents any atomic unit of work to be performed by our agents.
  - <u>**Connected Pattern**</u>: [trajectory](https://github.com/kastle-lab/modular-ontology-design-library/blob/master/modl/trajectory/trajectory-pattern.pdf), [sequence](https://github.com/kastle-lab/modular-ontology-design-library/blob/master/modl/sequence/sequence-pattern.pdf)
  - <u>**Source Dataset(s)**</u>: [ALFRED](https://askforalfred.com/), [RH20T-P](https://sites.google.com/view/rh20t-primitive/main)

---

- **Goal**

  - <u>**Rationale**</u>: Represents the desired outcome or terminal state toward which one or more tasks are directed; Anchors decomposition hierarchies and provides semantics for task sequencing order
  - <u>**Connected Pattern**</u>: [description-situation](https://github.com/kastle-lab/modular-ontology-design-library/blob/master/modl/description-situation/description-situation-pattern.pdf), [spatiotemporal-extent](https://github.com/kastle-lab/modular-ontology-design-library/blob/master/modl/spatiotemporal-extent/spatiotemporal-extent-pattern.pdf), [sequence](https://github.com/kastle-lab/modular-ontology-design-library/blob/master/modl/sequence/sequence-pattern.pdf), [event](https://github.com/kastle-lab/modular-ontology-design-library/blob/master/modl/event/event-pattern.pdf)
  - <u>**Source Dataset(s)**</u>: [BridgeData V2](https://rail-berkeley.github.io/bridgedata/), [EpicKitchens](https://epic-kitchens.github.io/2025), [RH20T-P](https://sites.google.com/view/rh20t-primitive/main), [ALFRED](https://askforalfred.com/)

---

- **Spatial**
  - <u>**Rationale**</u>: Captures the positional and relational information that constrains or enables the execution of tasks towards a goal within an avilable environment.
  - <u>**Connected Pattern**</u>: [spatial-extent](https://github.com/kastle-lab/modular-ontology-design-library/blob/master/modl/spatial-extent/spatial-extent-pattern.pdf), [spatial-object](https://github.com/kastle-lab/modular-ontology-design-library/blob/master/modl/spatial-object/spatial-object-pattern.pdf)
  - <u>**Source Dataset(s)**</u>: [Droid](https://droid-dataset.github.io/), [RH20T-P](https://sites.google.com/view/rh20t-primitive/main), [BridgeData V2](https://rail-berkeley.github.io/bridgedata/)

---

- **Category**

  - <u><b>Rationale</b></u>: Specifications to differentiate Spatial Things that are present within an environment.

  - <u>**Connected Pattern**</u>:

    - One major pattern that may suffice is the _explicit typing_ ODP, because one is describing an object by its _type_ or _category_: [Explicit Typing](https://github.com/kastle-lab/modular-ontology-design-library/tree/master/modl/explicit-typing).

  - <u>**Source Dataset(s)**</u>: [Princeton Model Net](https://modelnet.cs.princeton.edu/#)

---

- **Environment**

  - <u><b>Rationale</b></u>: Specifications to differentiate what is present/constitutes the environment in which a task is set/in which a robot(s) operates.
  - <u>**Connected Pattern**</u>:
    - Because an environment at its core consists of objects/things (zero, one, or many), all potentially related to one another, the [Part-whole (contextualized or not)](https://github.com/kastle-lab/modular-ontology-design-library/tree/master/modl/part-whole) may be the most appropriate.
    - Additionally, because an environment can consist of a list of objects, each with their descriptions, and a particular State, a highly modified integration of the _state transition_ and _sequence_ patterns may be appropriate. [State transition](https://github.com/kastle-lab/modular-ontology-design-library/tree/master/modl/state-transition), [Sequence](https://github.com/kastle-lab/modular-ontology-design-library/tree/master/modl/sequence).
  - <u>**Source Dataset(s)**</u>: [Droid](https://droid-dataset.github.io/)

---

- **Object**

  - <u><b>Rationale</b></u>: Specifications to define a non-autonomous Spatial Thing (not functional by itself).

  - <u>**Connected Pattern**</u>: Most likely the _spatial object_ or even the _spatiotemporal extent_ role would capture the qualities of an object, namely, that it occupies a position in space and time. [Spatial object](https://github.com/kastle-lab/modular-ontology-design-library/tree/master/modl/spatial-object), [Spatialtemporal extent](https://github.com/kastle-lab/modular-ontology-design-library/tree/master/modl/spatiotemporal-extent)

  - <u>**Source Dataset(s)**</u>: [Scanned Objects by Google](https://research.google/blog/scanned-objects-by-google-research-a-dataset-of-3d-scanned-common-household-items/), [BridgeData V2](https://rail-berkeley.github.io/)

---

- **Role**

  - <u><b>Rationale</b></u>: Used classify an agent’s immediate characteristics. To be distinct from the Archetype class as that is instead more representative of the culmination of all the characteristics an agent has based on their capabilities (i.e., a set of skills). The specific set of those capabilities gives an agent an archetype, allowing it to fill many roles until it is assigned to an immediate task, where it will fulfill a specific role.

  - <u>**Connected Pattern**</u>: [participant-role-pattern](https://github.com/kastle-lab/modular-ontology-design-library/blob/master/modl/participant-role/participant-role-pattern.pdf), [agent-role-pattern](https://github.com/kastle-lab/modular-ontology-design-library/blob/master/modl/agent-role/agent-role-pattern.pdf), [role-dependent-name](https://github.com/kastle-lab/modular-ontology-design-library/blob/master/modl/role-dependent-name/role-dependent-name-pattern.pdf)

  - <u>**Source Dataset(s)**</u>: TBD

---

- **Feature**

  - <u><b>Rationale</b></u>: A spatial thing that only exists as part of a host object (i.e., holes, color, bumps)

  - <u>**Connected Pattern**</u>: [Spatial-Object-Pattern](https://github.com/kastle-lab/modular-ontology-design-library/blob/master/modl/spatial-object/spatial-object-pattern.pdf)

  - <u>**Source Dataset(s)**</u>: [Scanned Objects by Google](https://research.google/blog/scanned-objects-by-google-research-a-dataset-of-3d-scanned-common-household-items/), [BridgeData V2](https://rail-berkeley.github.io/)

  ***

- **Geometry**

  - <u><b>Rationale</b></u>: The geometry data of a spatial thing (i.e., mesh data, dimensions)

  - <u>**Connected Pattern**</u>: [Spatial-Object-Pattern](https://github.com/kastle-lab/modular-ontology-design-library/blob/master/modl/spatial-object/spatial-object-pattern.pdf)

  - <u>**Source Dataset(s)**</u>: [Scanned Objects by Google](https://research.google/blog/scanned-objects-by-google-research-a-dataset-of-3d-scanned-common-household-items/), [BridgeData V2](https://rail-berkeley.github.io/)

---

- **RelationInstance**

  - <u><b>Rationale</b></u>: Through reification, typecasting properties into subproperties of a spatial thing (i.e., component, member, place, and feature types).

  - <u>**Connected Pattern**</u>: [Winston's Part Whole](https://ceur-ws.org/Vol-2195/pattern_paper_1.pdf)

  - <u>**Source Dataset(s)**</u>: All

---

- **SpatialThing**

  - <u><b>Rationale</b></u>: A physical thing that exists in time and space.

  - <u>**Connected Pattern**</u>: [spatial-object-pattern](https://github.com/kastle-lab/modular-ontology-design-library/blob/master/modl/spatial-object/spatial-object-pattern.pdf)

  - <u>**Source Dataset(s)**</u>: All
