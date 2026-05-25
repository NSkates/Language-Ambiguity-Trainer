# Language-Ambiguity-Trainer
This is a portion of the final exam project for CIS 379 (Systems Analysis and Design) that is able to be publicly shown (some portions of transcripts may be redacted, if necesarry). The transcripts in the LLM will be uploaded as an XML file.

The goal of this project is to train an LLM of choice to detect language ambiguity when given a set of data. The intention is not for the LLM to simply answer questions, but to demonstrate learned application of the framework in identifying ambiguity in new examples. The framework I plan to use to help me identify ambiguities is the dimensions of language quality as described in the journal article, Language Quality in Requirements Development: Tracing Communication in the Process of Information Systems Development by Christoph Rosenkranz, Marianne Corvera Charaf, and Roland Holten. The dimensions in this framework are dependent on being defined by the event’s symbols and actors. In the article, actors are essentially defined as a “representer.“ In other words, it’s someone (or sometimes, something) that gives the symbol a definition. A symbol could be defined as an entity that gets its meaning from the following actor. 

The article states the dimensions of language quality with the following: completeness, meaningfulness, non-redundancy, and unambiguity. The quality dimensions are based on how much meaning an actor is given. Due to this, completeness would be the best-case scenario for describing an actor because it’s “given when a representing symbol is given for every concept” (Rosenkranz, Christoph; Charaf, Marianne Corvera; Holten, Roland, 2013). Meaningfulness, on the other hand, is “given when every representing symbol is linked with one corresponding concept” (Rosenkranz, Christoph; Charaf, Marianne Corvera; Holten, Roland, 2013). If a quality dimension is non-redundant, then that’s because a group of single concepts all connect to one concrete symbol. No matter the linguistic unit. Finally, a quality dimension could be unambiguous. This happens “when no two concepts map into the same symbol” (Rosenkranz, Christoph; Charaf, Marianne Corvera; Holten, Roland, 2013).

Additionally, the LLM chosen for this project is ChatGPT.

The steps taken to train the LLM will be as followed:

1) Give the LLM context of its purpose
2) Define Language Quality Ontology
3) Identify instances of Language Quality Ontology
4) Define Few-Shot Prompting (so, it'll be quick to implement exemplars later in its training)
5) Inform LLM the framework it should use when finding ambiguities
6) Feed LLM additional relevant definitions and context related to the framework
7) Provide exemplars

The data the LLM will be working with a requirements list table for an Accounts Payable (AP) system. The data describing what the system should be able to do, not actual data output. There are two sections of the data we will be focusing on: Priority and Requirement. The Requirements describe the system's ability to perform a specific task. The Priorities describe how important that listed Requirement is. There are three kinds of Priorities, which are low, medium, and high. 

SOURCES
Rosenkranz, Christoph; Charaf, Marianne Corvera; and Holten, Roland (2013) "Language Quality in Requirements Development: Tracing Communication in the Process of Information Systems Development," Journal of Information Technology: Vol. 28: Iss. 3, Article 3.
DOI: 10.1057/jit.2012.33
Available at: https://aisel.aisnet.org/jit/vol28/iss3/3

