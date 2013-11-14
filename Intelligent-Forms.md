### baisc idea/motivation:

"Wikidata could be a lot smarter than it is right now e.g. by suggesting fields
to fill and probable values. 

For example: when an editor edits an item about a person that is still missing
the date of birth, this should be suggested as a possible property. Or when the
editor is entering the sex of the person, Wikidata should be smart and suggest
the ones that are used most for these properties first. Think of it as
something very similar to the famous 'people who bought x also bought y'
systems." (Quim Gil) - https://bugzilla.wikimedia.org/show_bug.cgi?id=46555

### assumptions/reflections:

There are two major use cases when it comes to suggesting properties:

1. Suggesting generally helpful properties for a newly created item 
Algorithms:
* Pairwise attribute cohesion table.* ...
2. Suggesting properties for an item based on its preexisting properties

### more detailed ideas regarding implementation:




