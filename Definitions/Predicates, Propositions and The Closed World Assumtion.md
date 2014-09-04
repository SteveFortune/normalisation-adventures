#Predicates and Propositions

A predicate is a function that turns true or false based on the values of its variables which may be a set. For example: `Everything in the set {1, 2, 3, 4} is a number between 0 and 5.`

A proposition is a statement which is either true or false based on what the result of a predicate on it is.

So…

	P(x)

- `P` is the predicate function
- `x` are the arugments of that function
- Parameters that substitute `x` are the proposition.
- The 'set' defined by the predicate (i.e. all the values of `x` for which `P(x)` is true) is denoted as `{x|P(x)}`


How does this relate to database design? We can take the attributes of a given relvar and use them as the arguments of the predicate. For example:

	A user has a first_name, has a last_name, has an email_address, has an age > 0 and < 100, and a telephone number with 11 numbers in it.
	
Here the relvar `user` represents the above predicate. Here are some propositions for the predicate:

_The predicate would return true for this proposition and thus the data described is a user_

	There is a user with the first_name of 'Ben', last_name of 'Wood', email_address of 'ben.wood@doglet.com', has an age of 19 and has a telephone number of '01453 833527'. 

_This proposition is false because the predicate would return false for it, and thus the data described is not a user_

	There is a user with the first_name of 'George', no last_name, no email_address and a telephone number of '1'. 

So for a given relation, every tuple represents a proposition. 


#The Closed World Assumtion

A given relvar at any given time contains only the tuples that that represent true propositions.

__TODO__ Elaborate



The following sources are helpful:

- http://yhcss.com/books/database_in_depth/databaseid-CHP-4-SECT-5.html
- http://en.wikipedia.org/wiki/Predicate_(mathematical_logic), 'Simplified Overview'