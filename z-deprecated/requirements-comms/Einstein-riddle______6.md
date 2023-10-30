# OPERATING NOTES
#### Numbering
I removed slide numbers to make it easier to reorder slides without having to renumber slides

## Rethinking "Main Idea"
The main idea is:
* How to find missing information?
* How to find missing information by connecting the dots?

In all of our examples, the information "is there" but it's not obvious, or - importantly - it has not **yet** been stated i.e. information that Google can present in search results.

We want to use the power of machine reasoning (the "computer") to present us with (find) hidden or undocumented information.

An over-used label here is "Artificial Intelligence".
We want to play off that concept - there's nothing 'artificial' about the information we need - it's just not readily apparent.

This is a very useful article:
* [Five levels of knowledge](https://enterprise-knowledge.com/beyond-find-the-five-levels-of-artificial-intelligence-for-knowledge/)

Five levels of knowledge:
* Answer
* Recommend
* Combine
* Infer
* Advise

You feature one of the types:
* recommend NetFlix movies based on your profile or viewing history

Einstein Riddle is:
* Infer - using information that "is there" but not apparent.

This was a good find (also an example of "Infer"):
* [Solving construction allocation problems](https://hrcak.srce.hr/file/252928) by minimizing allocation of fixed resources and reducing the time to construct a <building>

There is an answer but it's more challenging for a human to determine than a computer. 

#### I've made small changes below to capture the updated "Main Idea"

---

title: **Machines Can Think Logically Too**

# Slide: How to know ...
## Will my food conflict with my medicine?

## Will I like the flavor of a combination of specific foods and beverages?

See [see food compatibility](https://afdsi.com/___supplier/paula-perez/food-reaction) for ideas

## How do I find information about a product that is missing on its label?

    [Image: missing information about country-of-origin]

#### Attachment
Details about the above questions.

# Slide: Human Logic
## Humans use logic to connect the dots and make decisions.

### You use logical reasoning for simple problem solving, it’s a cognitive skill we benefit from is all kinds of situations. 

#### Attachment
[Logical reasoning](https://www.braingymmer.com/en/blog/logical-reasoning/)

# Slide: Machine Logic
## Machines use logic too, that is how they solve problems.

### Logic is one of the main components used in many common computer algorithms, such as the ones that decide what Netflix film you will want to watch next.

    [notes: see AI and levels of knowledge; has recommender systems]

#### Link
[Wikipedia Logic in computer science](https://en.wikipedia.org/wiki/Logic_in_computer_science)

# Slide: Einstein's Riddle
## We're going to show how to use machine logic to solve a famous riddle - the Einstein’s riddle

### This riddle focuses on deductive reasoning. With deductive reasoning, facts are used to come to a logical conclusion. If all the facts are true and all the rules of deductive logic are followed to come to a conclusion, then the conclusion will also be true.

#### Attachment
[Wikipedia Deductive reasoning](https://en.wikipedia.org/wiki/Deductive_reasoning)

# Slide: How the Riddle is organized
## Einstein’s riddle is a logic puzzle that gives sentences relating objects to each other.

There are five houses.
* The Englishman lives in the red house.
* The Spaniard owns the dog.
* Coffee is drunk in the green house.
* The Ukrainian drinks tea.
* The green house is immediately to the right of the ivory house.
* The Old Gold smoker owns snails.
* Kools are smoked in the yellow house.
* Milk is drunk in the middle house.
* The Norwegian lives in the first house.
* The man who smokes Chesterfields lives in the house next to the man with the fox.
* Kools are smoked in the house next to the house where the horse is kept.
* The Lucky Strike smoker drinks orange juice.
* The Japanese smokes Parliaments.
* The Norwegian lives next to the blue house.

# Slide: The question
## At the end, a question is asked on how certain objects related to each other. 

* Who drinks water?
* Who owns the zebra?

## Can you solve the Riddle?

    [Put a button link or a picture of the whole puzzle, so that people can pause and try to solve it, you can also include some image of the manual solution with the table]

# Slide: Components of the solution
## We will use three technologies to solve the riddle 

### An editor to organize the statements in computer format
### An ontology that makes the statements in the riddle
### A reasoner to solve the problem (find missing information)

# Slide: Protege
## An open system that uses these tools is Protege, developed by Stanford and free to use. If you want to explore how else you can use ontologies and reasoners, click here

### Protege screenshot

#### Attachment
Information about [Protege](https://protege.stanford.edu)

# Slide: Ontology
## Ontologies are detailed descriptions of something. For your purposes, think of an architect blueprint.

    [image of different nodes, similar to the computnet that you showed me]

### In the puzzle we gave at the beginning, the nationality (English, spaniard, ukranian) is a classified as a property of a person, where as the position (first, middle, etc. ) is associated with the house. Computers are able to create relationships between the different classes to determine which person lives in which house.

#### Attachment
[Wikipedia OWL](https://en.wikipedia.org/wiki/Web_Ontology_Language)

# Slide: Reasoner
## Reasoners are computer programs that are able to make connections between different objects in an ontology. For example, in our architect blueprint, which rooms should have a heater but do not.

    [image of lines appearing between the different nodes from the previous picture in slide 10]

### In our puzzle, if we know that the Englishman lives in the red house, we also know that he does not live in the blue house

#### Attachment
Information about [HermiT reasoner](http://www.hermit-reasoner.com)

# Slide: Steps to solve the Riddle
## So now, let’s look at how a computer would solve the riddle

Need to [summarize this page](https://afdsi.com/___supplier/story-einstein-riddle/einstein-riddle-description-OWL.html)

# Slide: Using Protege
## lead

![Set up in Protege](https://afdsi.com/___supplier/story-einstein-riddle/einstein-riddle-part-1.png)

# Slide: And the answer is ...
## lead

![Answer in Protege](https://afdsi.com/___supplier/story-einstein-riddle/japanese.png)
![Answer in Protege](https://afdsi.com/___supplier/story-einstein-riddle/norwegian.png)

And solved in 1 second

-----

# Slide: (uncertain)
## The computer creates different objects including the nationality, drink, pet and house of each person with the information available, and by using reasoners, fills in the gaps.

# Slide: Other applications
## Ontologies also have a wide variety of uses, from helping you choose your next Netflix movie, to more scientific applications like learning about cosmic relationships or helping doctors diagnose diseases.

#### Link
* https://www.datasciencecentral.com/ontologies-practical-applications/

