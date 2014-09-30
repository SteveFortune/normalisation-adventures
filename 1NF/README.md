#1NF

- Given that relation _R_ has attributes _A[1…n]_ of types _T[1…n]_ respectively, _R_ is in the first normal form if the value for attribute _Ai_ of tuple _t_ in _R_ has the type of _Ti (i=1, … n)_. 

- I.e. all tuples in a relation conform to the relation's heading, by having 1 value of the appropriate type for each attribute of the relation. 

- Every relation is in the first normal form by definition. A relation _R_ is _normalized_ if its in 1NF.

- In theory, an attribute could have a relational type (a _Relational Valued Attribute_).

- __Note__ because DBMSs don't properly support relvars (instead support _tables_), it possible for a database table _not_ be in 1NF. There are 5 requirements that are consequences of the fact that a relvar at a given time must have a relation value:

	1. No top to bottom ordering of the rows
	
	2. No left to right ordering of the columns
	
	3. No diplicate rows
	
	4. Every row and column intersection only contains one value of the applicable type. 
	
		- This means that _repeating groups_ or _multivalued attributes_ are not allowed
		- A column _C_ is defined as a repeating group if its defined to be in type _T_, however the values that appear in it are _groups_ (arrays, lists, sets, etc) of type _T_
	
		- Note that RVAs (noted above) are not repeating groups. __TODO__ Go in more detail about why (I'm still a bit confused about why this is, myself).
	
	5. All columns are regular, meaning that:
	
		- Every column must have a unique name in the table
		
		- Every row in the table can't contain anything beyond the column values (as required by 4.). 
		
		- I.e. there cannot be any 'hidden' or 'implicit' columns that can be only be accessed by 'special' operators.
		
		- I.e. there cannot be any columns that affect an invocation of a regular operator on a row, to have an irregular effect.
		
		- E.g. we cannot have identifiers that are not regular keys, like 'object IDs'
		
		- E.g. we cannot have hidden timestamp fields, like some [temporal databases](http://en.wikipedia.org/wiki/Temporal_database)