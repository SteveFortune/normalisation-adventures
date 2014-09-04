#Candidate Key

- A candidate key is a set of attributes that are unique such that every tuple in a relation has a unique set of values for each of its candidate keys. 
- The set of attributes that make up a candidate key may contain only 1 attribute.
- There can be multiple candidate keys for tuples in a relation.

Here are a few examples covering different cases of candidate keys…

###Example 1: Single Candidate Key as a Single Attribute

This example demonstrates a relation with a single candidate key. This candidate key is a set of just 1 attrbiute.

- We have a `User` domain
- A `User` has the following attributes: `email`, `first_name`, `last_name`
- `email` uniquely identifies the user
- `email` is the candidate key

###Example 2: Multiple Candidate Keys as Single Attrbiutes

This example demonstrates a relation with 2 candidate keys. These candidate keys are sets that contain just 1 attribute.

- We have a `User` domain
- A `User` has the following attributes: `email`, `username`, `first_name`, `last_name`
- `email` uniquely identifies a user
- `username` also uniquely identifies the user
- The relation has 2 separate candidate keys: `email` and `username`


###Example 3: Single Candidate Key as Multiple Attributes

This example demonstrates a relation with 1 candidate key. The candidate key is a set of 2 attributes that together are a unique pair that identify the relation.

- We have a `User` domain
- A `User` has the following attributes: `first_name`, `last_name`, `date_of_birth`, `telephone`
- In this application, the requirement is that only users with different names will sign up (a bit weird but hey..)
- A combination of `first_name` and `last_name` uniquely identifies a user
- `first_name, last_name` is the only candidate key



#Primary Key

The primary key is a candidate key that's been singled out and treated specially. Usually, if a relation has one candiate key then its designated as the primary key. If the relation has multiple candidate keys, the decision as to which one is the primary key based on which ever makes sense to the designer (one could argue that this decision is essentially arbirary).
