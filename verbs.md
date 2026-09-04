# Verbs

> A noun is a pattern preserved through change. A verb is the change through which patterns persist, reproduce, interact or disappear.

## Status

This is an exploratory note, not a finished ontology and not a proposal to enlarge the Village Link primitive.

## Berners-Lee: nodes and predicates

The first-page diagram in Tim Berners-Lee's 1989 [*Information Management: A Proposal*](https://cds.cern.ch/record/369245/files/dd-89-001.pdf) mixes people, documents, organisations, technologies and concepts as nodes. Its arrows carry labels such as *describes*, *includes*, *refers to*, *wrote* and *unifies*.

Berners-Lee later says that a node should ideally represent or describe a particular person or object. His examples include people, software modules, groups, projects, concepts, documents, and types and instances of hardware. He says that the circles and arrows may stand for anything and that useful systems should recognise generic node and link types without imposing limitations.

He does not literally formulate this as **any noun connected by any verb**, but that is a fair compression of the architecture. A later [W3C reconstruction of the diagram in RDF](https://www.w3.org/1999/11/11-WWWProposal/) describes the arrows as typed links or properties among named objects.

There is, however, an important distinction between these predicates and verbs in the deeper sense considered here.

## Predicates describe a graph; verbs change it

A labelled edge in a knowledge graph usually expresses a proposition:

> Joe — works for → Inky Tech

This describes a relationship in a particular state of the world. It does not itself make anything happen.

An event such as:

> Joe joins Inky Tech

changes the graph by creating that relationship. A later event:

> Joe leaves Inky Tech

changes it again.

The earlier Village Link possibility:

> [A][Operator][B]

would therefore have supplied a broad vocabulary of typed **predicates**: *employs*, *owns*, *wrote*, *loves*, *killed*. Although many predicate labels look grammatically like verbs, they remain assertions about how a graph stands.

A verb in the stronger sense is an event, process or operation that transforms the graph:

```text
world state at time t
        |
      verb
        |
world state at time t + 1
```

Or more formally:

```text
(pattern, environment)t -- verb --> (pattern', environment')t+1
```

Predicates describe a state. Verbs introduce the time dimension.

## Nouns, verbs, constraints and consequences

A provisional division is:

| Concept | Fundamental meaning |
| --- | --- |
| Noun | A pattern recognisable across time |
| Verb | A transformation involving that pattern |
| Constraint | What transformations are possible, costly or forbidden |
| Consequence | How a transformation affects persistence or reproduction |
| Fitness landscape | The structured field of constraints and consequences encountered by possible patterns and behaviours |

A verb may be something a pattern does—*eats*, *copies*, *cooperates*, *lies*—or something that happens to it—*breaks*, *mutates*, *dies*, *is remembered*. Agency is not required. What matters is change.

This suggests that a fitness landscape is not merely a set of constraints. It also contains the consequences attached to possible verbs.

A cliff constrains where a gazelle can run. A lion gives running one set of consequences and standing still another. Evolution operates on the resulting history of events: ran, escaped, ate, mated, reproduced.

The fitness of a noun is therefore shorthand for something dynamic:

> How successfully does this pattern's repertoire of verbs perpetuate the pattern in this landscape?

Nouns are the invariants we recognise across transformations. Verbs are the transformations.

## Information executes as verbs

Information does not survive merely by sitting in the world as a noun. Successful information causes events:

> Copy me. Remember me. Teach me. Obey me. Build this. Punish defectors. Tell the children.

Genes and memes are not only descriptions. They are instructions that obtain machinery, energy and media through which they can be executed and copied.

This sharpens the idea of the village as a general-purpose machine. The current condition of its people, artefacts, environment and memory is its state. Its cultural programs supply rules that help produce the next state. Institutions are durable arrangements of permitted, required, rewarded and punished verbs.

The evolutionary question is therefore not only which informational patterns exist, but what those patterns cause their hosts and environments to do.

## Relationship to Village Link

This line of thought does not reopen Village Link's equality-only decision.

Village Link connects traces in independently governed memory systems that refer to the same noun:

> P asserts A ↔ B

That is identity infrastructure. A system wishing to represent events must first know which Joe, which organisation, which document and which earlier event it is talking about. The noun layer is a prerequisite for a reliable verb layer.

The verb layer, if one is eventually required, belongs above or beside Village Link rather than inside its primitive.

Nor is there a contradiction when a relationship or event is later treated as a noun. Once reified, a record of an event can acquire identifiers, evidence and relationships of its own. The important discipline is to keep the descriptive levels clear:

- a predicate describes a relationship in a graph;
- a verb transforms the graph;
- a record of either may itself become a noun in a higher-order graph.

## Questions

This distinction opens a substantial field of work:

- Is a verb best modelled as an observed event, a possible transition, an executable rule, or all three?
- What is the relationship between action, process, event and causation?
- Which verbs are initiated by an agent, and which merely happen to a pattern?
- How do norms and institutions alter the set and consequences of available verbs?
- Is culture best understood as stored information, executable programs, histories of execution, or some combination?
- Does selection operate chiefly on nouns, or on repertoires of verbs that allow patterns to persist and reproduce?
- How should time, sequence and counterfactual possibility be represented without collapsing back into an unrestricted knowledge graph?

For now, the central distinction is:

> **Predicates describe the graph. Verbs change the graph.**
