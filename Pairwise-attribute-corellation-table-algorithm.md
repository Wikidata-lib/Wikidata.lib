todo: graphics

##  Prepare static data
1. Create a table:
  Theres a column and a line for each property in wikidata.
2. Fill in table:
  Iterate through all items i and:
  step through all properties p contained in i
  * globally count appearances of p a 1D Array
  step through all pairs of properties (p,q) contained in i
  * globally count appearances of (p,q) in Table from (1.)
3. Compute (appearance of (p,q)) / ((appearance of p)+(appearance of q))

## Compute attribute ranking for certain set of properties
Ma = certain set of properties.

the rank for a property p = for each x in Ma multiply: (p,x)


