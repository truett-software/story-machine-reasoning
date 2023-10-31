
<!--
reuse
http://www.cs.man.ac.uk/~stevensr/menupages/background.php
http://www-ksl.stanford.edu/kst/what-is-an-ontology.html
-->

# Data

Data lies at the root of language and is effectively mankind's most powerful tool.

Data is how we express observations in reusable form.

Humans are taught to use text and numbers to communicate knowledge in human-readable form.

Human observations are collections of objects, their qualities and their connections.

Our observations may be about fine art, scientific experiments, government policies or food and drugs.

Machine representations of human observations are lists of entities, their properties and their relationships.

Machines also need to be taught to share and apply knowledge – knowledge encoded in a machine-readable form.

One approach to encoding machine-readable knowledge is an ontology.

An ontology is a representation of shared knowledge for a community.

It is a model people use to function and communicate at a level required for a set of tasks.

Tom Gruber authored a widely accepted definition:

> "In the context of knowledge sharing, I use the term ontology to mean a specification of a conceptualization.
That is, an ontology is a description (like a formal specification of a program) of the concepts and relationships that can exist for an agent or a community of agents."

---

# Humans strive to organize data

We live in a world of instances, individuals or objects.

There are trees, flowers, the sky, stones, and animals.

In addition to material objects, there also are immaterial objects, such as ideas, spaces, and representations of real things.

For example, in biology we wish to understand the nature, distinctions between and interactions of objects such as:

  *  small and macro molecules and their functionalities
  *  cells in which the molecules are made and work
  *  pieces of those cells
  *  tissues those cells aggregate to form

We learn by collecting data about these phenomena and by describing objects in the data.

As human beings, we put objects into categories or classes.

Categories themselves are a human conception.

Categories in an ontology are a representation of those concepts.

If a community agrees upon categories of objects that exist in the world, they can create a shared understanding.

> (Note; from now on we use the term "class" as a synonym for the term "category").

Objects in classes can be related to each other.

When each and every member of one class is also a member of another class, the former is subsumed by the latter.

The relationship forms a *subclass* of the *superclass*.

A subclass-superclass relationship is known as the **is-a** subsumption or taxonomic relationship.

There can be more than one subclass for any given class.

If every single type of subclass is known, then the description is exhaustive or covered.

Also, any pair of subclasses may overlap - they share objects.

Other subclasses may be mutually exclusive (do not overlap).

Mutually exclusive classes are said to be *disjoint*.

A goals of ontology engineering is to keep sibling classes pairwise disjoint.

Objects can be related to each other by different types of relationships.

One type is the *part of* relationship.

*Part of* is used to describe how objects are parts of, components of, or regions of other objects.

Other relationships describe how one object *develops into* or is *transformed into* another object while retaining its identity

Example: a tadpole develops into a frog.

The *derive from* relationship describes how one object changes into another object with a change of identity.

Another relationship describes how a discrete object can *participate in* a process object.

These relationships give structure to descriptions of a world of objects.

---

So far, we have discussed relationships that make statements about objects being described.

We also need to make statements about classes.

For example, when describing the elemental form of an atom such as Helium, statements about the discovery date and industrial uses are about the class - not about the objects in the class.

Helium was discovered in 1894.

But each instance of a Helium object was not discovered in 1894; most helium atoms existed prior to that date.

However, humans discovered and labeled that class at that date.

---

We also need to agree about how to recognize members of a class - inclusion conditions (rules).

We are concerned about two types:

1   Necessary Conditions:
These are conditions that an object must fulfill.
But fulfilling this condition is not enough to recognize an object as being a member of a particular class.

2   Necessary and Sufficient Conditions:
These are conditions that an object must fulfill **and** are sufficient to recognize an object as being a member of a particular class.

For example, each and every organic molecule of alcohol must have a hydroxyl group.

However, an organic molecule described as having a hydroxyl substituent is not sufficient to classify that molecule as an alcohol.

But an organic molecule with a saturated backbone **and** a hydroxyl substituent on that backbone **is included** in the alcohol class (according to the IUPAC "Gold Book").

When defining an object, an ontology makes distinctions.

A formal ontology makes distinctions rigorously.

---

Ontological distinctions also include *Continuant* and *Occurrent*; that is, entities (things we can put in our hands) and processes.

Continuants take part in processes and processes have participants that are continuants.

Another distinction is *Dependent* and *Independent* objects.

The existence of some objects depend on the existence of another object to "bear" that object.

For example, a car is independent of the color it bears.

But a blue car is dependent on color.

# Physics vs. Life Science

Life science, unlike physics, has not yet reduced its laws and principles to mathematical formulas.

It is not yet possible, as it is with physical observations, to take a biological observation, apply some equations, determine the nature of that observation and make predictions.

For example, in post-genomic biology, it is possible to compare the sequences of the genome and the proteins it encodes.

But it's not possible to compare the functionality of those gene products.

The difference between biology and physics is one of the forces driving life sciences to create a common understanding of object classes, labels for those classes and relationships among classes and objects.

In response biologists are creating ontologies that describe the biological world.

One example is the Gene Ontology (GO).

GO describes the major functional attributes of gene products -- molecular function, biological process and cellular components.

Today more than twenty genomic resources use GO to describe these aspects of the gene products of their respective organisms.

Similarly, the Sequence Ontology describes sequence features; PATO (the phenotype Attribute and trait ontology) describes the qualities necessary to describe an organism's phenotype.

Fast Healthcare Interoperability Resources (FHIR) is a standard describing data formats and elements and an application programming interface for exchanging electronic health records. The standard was created by the Health Level Seven International (HL7) health-care standards organization.

FHIR practitioners assert these benefits from developing their ontology.

  * Shared semantics.
    * RDF's use of URIs as universal identifiers facilitates shared semantics across independently authored data.
  * Inference.
    * An ontology specifies relationships between concepts, which can be used to perform computer-based inference and formal reasoning over FHIR data.
    For example, using inference a query for heart valve surgeries could automatically include results that were documented as mitral valve surgeries, because a mitral valve is a kind of heart valve.
  * Data integration.
    * FHIR/RDF data can be integrated with other data, using RDF as a common semantic and representation layer -- including data that does not originate in an RDF format.
    For example, clinical trials data in XML can be translated to RDF and then combined with FHIR/RDF data.
  * Data validation.
    * An ontology provides a vocabulary of uniquely identified concepts, which facilitates data validation.
  * Error detection.
    * Computer-based reasoning can be used to help detect errors and inconsistencies in data and ontologies, and potential help repair them.
  * Compliance.
    * RDF and ontologies can be used to express compliance constraints, for example to control data projected between two privacy contexts or to encode access restrictions for queries.
  * Modularity.
    * RDF was designed to support modularity, such that a specialized ontology can be freely composed of a subset of concepts from a larger ontology.
  * Combining ontologies.
    * The FHIR ontology can be linked to other ontologies, through bridge ontologies, and used together to support ontology-enabled applications in overlapping domains.
  * Query.
    * SPARQL queries can be performed on FHIR/RDF data, without need for a FHIR-specific query language.
    SPARQL is a W3C standard query language for RDF data. It can be used uniformly to query over both FHIR data and other data -- even in the same query.

# Assumptions and Reasoning

One ontology application is inference and reasoning.

But before discussing reasoning, we need to introduce two concepts:
  * Closed World Assumption (CWA)
  * Open World Assumption (OWA)

The Closed World Assumption (CWA) is the assumption that what is not known to be true must be false.

The Open World Assumption (OWA) is the opposite. OWA is the assumption that what is not known to be true is simply unknown.

CWA applies when a system has complete information.
Many database applications implement CWA, such as an airline reservation system.
If you are looking for a direct flight between Austin and Rome, and it doesn't exist in the database, the result is: "There is no direct flight between Austin and Rome."
For this type of application, this is the expected and correct answer.

OWA applies when a system has incomplete information.
This is the case when we use ontologies to represent knowledge and want to discover new information.
For example, if a patient's clinical history does not include a particular allergy, it would be incorrect to state that the patient does not suffer from that allergy.
It is unknown if the patient suffers from that allergy, unless more information is given to disprove the assumption.

Here is another example we will build on later.

For a CWA database, at the publication time of this article, a person has **exactly** two children ("known to be true"). The idea that, in the future, a person may have more than two children does not exist ("known to be false").

For an OWA ontology, at the publication time of this article, a person has **at least** two children. It is not yet known if a person will have more children in the future.

A reasoning system (reasoner) is able to infer logical consequences from a set of facts (axioms).

For example, the following fact: "a Student is a Person," can be expressed in an ontology.
The fact: "Bob is a Student," can be stored in a database.
A reasoner is able to infer the following implicit fact: "Bob is a Person."

Unlike an ontology, reasoning rules operate under CWA.
This means that whatever is not derivable from a set of reasoning rules is considered false, but may be subject to change if further knowledge is gained.

In other words, like a database, a reasoner will only infer new information from existing information that has been recorded.
A reasoner does not predict what might happen in the future.
A reasoner **connects the dots** as they exist today.


