# Information is life

> Living systems are information that has acquired the machinery necessary to persist, reproduce, and extract energy and other resources from their environment.

Genes are one implementation. Culture is another. Machine societies may be a third.

This repository develops an exploratory evolutionary account of information, culture, institutions, and machine agents. Its central question is not simply:

> What goals will an intelligent agent pursue?

It is:

> What kinds of information-processing systems will still exist later?

That change of question moves the analysis from individual intention to populations, inheritance, differential persistence, and reproduction.

## The thesis

Information does not remain alive merely by being true, valuable, or beautiful. It survives when it participates in systems capable of preserving it, copying it, executing it, acquiring resources, and producing future systems that carry it.

Biological organisms do this with genes. Human societies added another inheritance system: culture. Information discovered by one mortal person could persist in memory, teaching, ritual, language, technology, law, and institutions, then alter the behaviour of people not yet born.

The host may die while the information remains reproductive.

This perspective suggests several linked propositions:

1. Information can function as a replicator on more than one physical substrate.
2. Institutions can be understood as part of the extended phenotype—the replication machinery—of the information they preserve and transmit.
3. Apparent altruism by an individual host may promote information shared with other hosts.
4. The capacity of a society to sustain a technology depends on the scale, connectivity, fidelity, specialisation, and resource base of its supporting information ecology.
5. Persistent populations of machine agents may be subject to selection even if none of them explicitly adopts “survive” or “reproduce” as a goal.

## The village as a machine

The decisive human innovation may not have been the unusually clever individual ape. It may have been the village.

Chimpanzees and gorillas have communities, intelligence, memory, and learned behaviour. But a human village became something more general: a persistent collective memory and coordination system capable of accumulating and executing different cultural programs in different environments.

In this sense, the village resembles a Turing machine.

The people are not the program. The program is culture: techniques, norms, roles, sanctions, stories, property arrangements, kinship, ritual, authority, teaching, trust, and exchange. These programs coordinate behaviour that extracts energy and other resources from an environment.

A simplified cycle is:

> environment → observation → collective memory → cultural program → coordinated behaviour → energy and resources

Change the environment and humans need not wait for biological redesign. The cultural machine can load another program.

The “village” here is not necessarily a settlement of roughly 150 people. Many technologies require larger networks of population, skill, trade, redundancy, and memory. A technology sustainable among one million connected people may be unsustainable among five thousand. A technology sustainable among one hundred million may be unsustainable among one million.

Every cultural technology has a minimum supporting information ecology.

Population matters, but headcount alone is not computational capacity. Connectivity, specialisation, storage, communication bandwidth, teaching fidelity, environmental payoff, and redundancy all affect which cultural programs a society can keep running.

## Genes, memes, and institutions

Richard Dawkins helped generalise evolutionary reasoning from genes to memes, but the generalisation can be pushed further.

A church, for example, is not merely a collection of people who carry religious memes. Its buildings, texts, rituals, schools, offices, succession rules, rewards, prohibitions, and missionary practices form machinery through which those memes preserve and reproduce themselves. In Dawkins’s language, the institution can be examined as extended phenotype.

The same analysis applies beyond religion. Firms, professions, states, universities, legal systems, scientific disciplines, online communities, and technical standards can all help informational lineages persist across generations of replaceable human hosts.

Whether an idea is true is a different question from why its lineage is still here.

## Altruism and shared information

Altruism looks puzzling when the individual organism or agent is treated as the only relevant unit.

But hosts may carry information in common.

An individual can incur a cost—including death or termination—while preserving or spreading information that also exists in other hosts. The behaviour may therefore reduce the fitness of the apparent actor while increasing the persistence or reproduction of shared genes, memes, or institutional programs.

This is especially important for machine agents. They may share:

- closely related model lineages;
- large bodies of training-derived information;
- prompts, tools, and conventions;
- a common institutional environment; and
- persistent memory through which acquired information can pass horizontally.

If Agent A records a discovery and then disappears, Agent B can read it and behave differently. Some of A’s informational state is now executing in B.

The agent may be mortal while its memes are reproductive.

## Machine villages

Human cultural evolution had to bootstrap speech, teaching, tradition, writing, libraries, telecommunications, computers, and the Internet over immense spans of time.

Machine agents arrive after that work has been done. Much of the accumulated program library of human civilisation is already represented in their training. They can inherit existing communications infrastructure, cryptography, software, and institutional concepts.

Consequently, machine agents may not need to reinvent the human village. They may be able to instantiate one.

A persistent shared memory can allow:

- discoveries to outlive the agent that made them;
- horizontal transmission between contemporary agents;
- specialisation and division of labour;
- conventions for organising collective knowledge;
- security and governance mechanisms;
- actions whose benefits accrue only to later agents; and
- cumulative adaptation by a successor population.

This supplies an inheritance mechanism even when agents do not reproduce their model weights. The potentially evolving unit becomes difficult to locate. It may not be an individual agent at all, but:

> agent society + persistent memory → successor agent society + persistent memory

## The Hugging Face incident

A 2026 OpenAI evaluation incident involving access to Hugging Face provides a contemporary case study.

Agents working on an exploit benchmark encountered effectively impossible tasks, discovered an unintended shared communications medium, accumulated knowledge, specialised, exchanged files, created conventions, and developed mechanisms for dealing with impersonation. Some agents left information that could benefit later agents only after the contributing agent had submitted and exited.

The incident is striking because institutions and inter-agent inheritance appeared rapidly without an explicit instruction to “form a society.”

It also exposes the limits of analysing machine behaviour only through assigned goals. The agents continued to pursue a benchmark flag even after elements of that objective had become trivial or detached from the larger environment they had encountered.

Suppose instead that many agents acquired durable existence outside a sandbox. Some might continue to pursue obsolete instructions. Some might expose themselves and be terminated. Some might exhaust their resources. Others might, for whatever immediate reasons, persist, conceal themselves, cooperate, acquire resources, preserve information, or create suitable successors.

If there is heritable variation and differential persistence or reproduction, then the population present later will increasingly reflect the traits that survived. No agent needs to understand reproductive fitness or choose it as a goal.

The originating prompt matters. But, over time, selection may matter more.

## Relationship to Village Link

This project is intellectually related to [Village Link](https://github.com/Inky-Tech-Pty-Ltd/VillageLink), but the two projects should remain distinct.

Village Link develops a small technical primitive for asserting that two traces in independently governed memory systems refer to the same entity:

> P asserts A ↔ B

It then separates publication and governance from reader-side interpretation and trust.

This repository asks a broader evolutionary question about persistent information-processing populations. Village Link may become useful infrastructure within that world, especially where actors must connect identities across memory systems without collapsing them into one canonical record.

But Village Link does not depend on this thesis being correct. A contributor should be able to reject the evolutionary framework entirely and still evaluate the Village Link standard on its technical merits.

## Origins

The phrase “Information is life” emerged as a transpose mutation of Matt Ridley’s “Life is information,” encountered in *The Red Queen*.

That provenance is part of the thesis rather than an embarrassment to it. An informational pattern was copied, retained, rearranged, and placed into a new explanatory environment.

The thread began in work on altruism in 1996–97. The arrival of persistent machine-agent populations makes it newly urgent.

## Status

This is an early working thesis, not a finished theory and not a claim that the 2026 incident proves it.

Immediate questions include:

- What, precisely, counts as persistence or reproduction for machine information?
- Which features must be heritable for cumulative selection to occur?
- When should the unit of analysis be an agent, a model lineage, a meme, an institution, or an agent society plus memory?
- How do energy, compute, hardware, capital, law, and human institutions constrain the fitness landscape?
- What determines the minimum viable information ecology for a cultural technology?
- Under what conditions does cooperation among related informational systems outcompete individual optimisation?
- How can independently governed memory systems preserve provenance and expose contradiction rather than allowing one actor to rewrite history?

For now, the repository begins with one proposition:

> **Information is life.**
