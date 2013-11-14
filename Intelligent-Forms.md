### baisc idea/motivation:

"_Wikidata could be a lot smarter than it is right now e.g. by suggesting fields__
_to fill and probable values._

_For example: when an editor edits an item about a person that is still missing_
_the date of birth, this should be suggested as a possible property. Or when the_
_editor is entering the sex of the person, Wikidata should be smart and suggest_
_the ones that are used most for these properties first. Think of it as_
_something very similar to the famous 'people who bought x also bought y'_
_systems._" (Quim Gil) - https://bugzilla.wikimedia.org/show_bug.cgi?id=46555

### assumptions/reflections:

There are two major use cases when it comes to suggesting properties:

**1) Suggesting generally helpful properties for a newly created item**

Even though an official ontology for the items in wikidata does not exist, there are still "classifying" properties/classifiers (e.g InstanceOf, SubclassOf, memberOf etc.) having classes as their values.
Items that belong to the same class often by nature have a lot in common. This makes knowing an item's classifiers and their concrete values very useful for suggesting properties.
Therefore a selection of widely used/important classifiers could be suggested as initial properties to a users that wants to create a new item. The idea is that after the property value was filled in, the user can profit from the derived suggestions during further editing.

Since there are no predefined/fixed classifiers the first step is to find a way to identify properties that serve as classifiers - a few thoughts regarding this issue:
* Only properties with the item type should be considered a potential classifier due to the fact that a class thatr is used as the value for a classifier is most likely going to be represented by an item in wikidata

**2) Suggesting properties for an item based on its preexisting properties**

Algorithms:
  * [Pairwise Attribte Correlation Table Algorithm ](https://github.com/Wikidata-lib/Wikidata.lib/wiki/Pairwise-attribute-corellation-table-algorithm)
  * ...

### more detailed ideas regarding implementation:




