# Key Notions

What entities you think would exist in your graph?

- **Capability**
  - <u><b>Rationale</b></u>: Specifications to differentiate and define an agent is capable of doing.
  - <u>**Connected Pattern**</u>: [role-dependent-name](https://github.com/kastle-lab/modular-ontology-design-library/tree/master/modl/role-dependent-name),
  - <u>**Source Dataset(s)**</u>: [Droid](https://droid-dataset.github.io/)

---

- **Agent**
  - <u>**Rationale**</u>: rationale
  - <u>**Connected Pattern**</u>: [agent-role](https://github.com/kastle-lab/modular-ontology-design-library/blob/master/modl/agent-role/agent-role-pattern.pdf)
  - <u>**Source Dataset(s)**</u>: [RH20T-Ps](https://sites.google.com/view/rh20t-primitive/main)

---

- **Event**
  - <u><b>Rationale:</b></u> Capturing the specific **things that just happened** at a certain point of time, like when robot gripper confirms it has successfully picked up its target. This event is the trigger that causes the robot's State to change from executing to idle, signaling the orchestrator that the step is complete and it can now issue the next Task in a sequence.
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

- **Key Notion**
  - <u>**Rationale**</u>: rationale
  - <u>**Connected Pattern**</u>: pattern name (pattern source)
  - <u>**Source Dataset(s)**</u>: dataset n, dataset n+1

---

# Identified Key Notions and Associated Potential MODL Patterns

## Chris

- Tasks
- Goal
- Spatial
- Provenance

## Susan
- Namestub
- Events
- Environment
- Temporal

## Shreyas

- Categorization
- Environment
- Objects

## Michael

- Provenance
- Archetype
- Agents
- States
- Capabilities

### Agents

- [agent-role](https://github.com/kastle-lab/modular-ontology-design-library/blob/master/modl/agent-role/agent-role-pattern.pdf)

### Capabilities

- [role-dependent-name](https://github.com/kastle-lab/modular-ontology-design-library/tree/master/modl/role-dependent-name)

### Objects

- [description-situation](https://github.com/kastle-lab/modular-ontology-design-library/blob/master/modl/description-situation/description-situation-pattern.pdf)

- [spatial-object](https://github.com/kastle-lab/modular-ontology-design-library/blob/master/modl/spatial-object/spatial-object-pattern.pdf)

### Events

- [event](https://github.com/kastle-lab/modular-ontology-design-library/blob/master/modl/event/event-pattern.pdf)

- [description-situation](https://github.com/kastle-lab/modular-ontology-design-library/blob/master/modl/description-situation/description-situation-pattern.pdf)

- [causal-event](https://github.com/kastle-lab/modular-ontology-design-library/blob/master/modl/causal-event/causal-event-pattern.pdf)

- [recurrent-event](https://github.com/kastle-lab/modular-ontology-design-library/blob/master/modl/recurrent-event/recurrent-event-pattern.pdf)

### Task

- [sequence](https://github.com/kastle-lab/modular-ontology-design-library/blob/master/modl/sequence/sequence-pattern.pdf)

### State

- [state-transition](https://github.com/kastle-lab/modular-ontology-design-library/blob/master/modl/state-transition/state-transition-pattern.pdf)

### Goals

- See tasks

### Environment

- See events
- See objects
- [observation](https://github.com/kastle-lab/modular-ontology-design-library/blob/master/modl/observation/observation-pattern.pdf)

### Priority

- TBD

### Classification/Category

- TBD

### Archetype (role)

- [explicit-typing](https://github.com/kastle-lab/modular-ontology-design-library/blob/master/modl/explicit-typing/explicit-typing-pattern.pdf)

- [participant-role](https://github.com/kastle-lab/modular-ontology-design-library/blob/master/modl/participant-role/participant-role-pattern.pdf)

### Temporal

- [temporal-extent](https://github.com/kastle-lab/modular-ontology-design-library/blob/master/modl/temporal-extent/temporal-extent-pattern.pdf)

### Spatial

- [spatial-extent](https://github.com/kastle-lab/modular-ontology-design-library/blob/master/modl/spatial-extent/spatial-extent-pattern.pdf)

- [spatiotemporal-extent](https://github.com/kastle-lab/modular-ontology-design-library/blob/master/modl/spatiotemporal-extent/spatiotemporal-extent-pattern.pdf)

### Other

- [name-stub](https://github.com/kastle-lab/modular-ontology-design-library/blob/master/modl/name-stub/name-stub-pattern.pdf)

- [provenance](https://github.com/kastle-lab/modular-ontology-design-library/blob/master/modl/provenance/provenance-pattern.pdf)

---
