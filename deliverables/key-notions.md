# Key Notions

What entities you think would exist in your graph?

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
  - <u>**Rationale**</u>: To identify which multi-agent (MAS) system a robotic agent originates from.
  - <u>**Connected Pattern**</u>: [provenance](https://github.com/kastle-lab/modular-ontology-design-library/blob/master/modl/provenance/provenance-pattern.pdf)
  - <u>**Source Dataset(s)**</u>: TBD

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
