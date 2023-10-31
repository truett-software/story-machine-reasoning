# Reasoners

Reasoners are computer programs that can infer logical consequences from a set of facts (axioms), which are usually the data stored in an ontology.

For example, the following fact: "a Student is a Person," can be expressed in an ontology. The fact: "Bob is a Student," can be stored in a database. A reasoner is able to infer the following implicit fact: "Bob is a Person."

But before discussing reasoning, we need to introduce two concepts:
  * Closed World Assumption (CWA)
  * Open World Assumption (OWA)

CWA is the assumption that what is not known to be true must be false. This is applied when a system has complete information, such as airline reservation systems.

OWA is the opposite. OWA is the assumption that what is not known to be true is simply unknown. It applies when a system has incomplete information. For example, if a patient's clinical history does not include a particular allergy, it would be incorrect to state that the patient does not suffer from that allergy.

Unlike an ontology, reasoning rules operate under CWA.

This means that whatever is not derivable from a set of reasoning rules is considered false, but may be subject to change if further knowledge is gained.

In other words, like a database, a reasoner will only infer new information from existing information that has been recorded.

A reasoner does not predict what might happen in the future.

A reasoner **connects the dots** as they exist today.



