# What is an Ontology?

Data is how we express our observations about fine art, scientific experiments, government policies or food and drugs, and is effectively mankind's most powerful tool. As humans, we use text and numbers to communicate this data in a way that other people would understand. 

Machine use a different language to express data. They use lists of entities, their properties and their relationships in order to understand human observations. A way to encode this knowledge in a machine-readable way is called an ontology. 

Tom Gruber authored a widely accepted definition for ontology:

> "In the context of knowledge sharing, I use the term ontology to mean a specification of a conceptualization. That is, an ontology is a description (like a formal specification of a program) of the concepts and relationships that can exist for an agent or a community of agents."

# How is information stored in an ontology?

As human beings, we put objects into categories. 

Similarly, ontologies use classes to store objects. Objects in classes can be related to each other. 

There are also subclasses, when each and every member of one class is also a member of another class. There can be more than one subclass for any given class.

When two classes do not have any element in common, they are called *disjoint*. A goal of ontology engineering is to keep sibling classes pairwise disjoint.

# How are objects' relationships stored?

Objects can be related to each other by different types of relationships.

Other relationships describe how one object *develops into* or is *transformed into* another object while retaining its identity.

One type is the *part of* relationship.*Part of* is used to describe how objects are parts of, components of, or regions of other objects.

Another relationship is the *derive from*. The *derive from* relationship describes how one object changes into another object with a change of identity.

Another relationship describes how a discrete object can *participate in* a process object.

These relationships give structure to descriptions of a world of objects.

# How to describe an object or class?

We also need to make statements about classes. For example, Helium was discovered in 1894.

When describing the elemental form of an atom such as Helium, statements about the discovery date and industrial uses are about the class - not about the objects in the class.

# How to recognize an object or class?

We also need to agree about how to recognize members of a class - inclusion conditions (rules).

We are concerned about two types:

1. Necessary Conditions. These are conditions that an object must fulfill. But fulfilling this condition is not enough to recognize an object as being a member of a particular class.

2. Necessary and Sufficient Conditions. These are conditions that an object must fulfill **and** are sufficient to recognize an object as being a member of a particular class.

For example, each and every organic molecule of alcohol must have a hydroxyl group.

However, an organic molecule described as having a hydroxyl substituent is not sufficient to classify that molecule as an alcohol.

But an organic molecule with a saturated backbone **and** a hydroxyl substituent on that backbone **is included** in the alcohol class (according to the IUPAC "Gold Book").

When defining an object, an ontology makes distinctions.

That is why a formal ontology needs to make distinctions rigorously.
