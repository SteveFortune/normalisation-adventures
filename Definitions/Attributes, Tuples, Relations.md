#Attributes

An attribute is a specification describing the property of an object. For example we may have a `Thing` `class` which contains a `public String name;` property. Here the attribute is a `String` called `name` that we attribute to an instance of a `Thing` object.


#Tuples

A tuple is an ordered list of elements. For example, in a database we may have a `Thing` table. Its attributes are defined as its columns: `name`, `colour`, `smell`, `shape`. 

An row in the `Thing` table could be describes as a tuple: `(England, Mostly Green, Tea and Disapointment, Kind-of-like-a-boot)`. An ordered list of elements which in this instance, describe a `Thing`.


#Relations

A relation is a set of tuples that are part of a specific data domain. 

Back to the `Thing` table, we have a data domain described by the columns: `name`, `colour`, `smell`, `shape`. A relation would be lots of tuples in this table (i.e. a set of tuples), e.g.


- `(England, Mostly Green, Tea and Disapointment, Kind-of-like-a-boot)`
- `(Apple, Red, Fruity, Round)`
- `(Person, Pink, Sweat, Generally Tubular)`


[This diagram](http://en.wikipedia.org/wiki/Relation_(database)#mediaviewer/File:Relational_database_terms.svg) was really helpful for me to visualise how these concepts apply to relational database design.


###Relation Variables

A relational variable is a relation that changes over time. E.g. in a database we have a `User` table. At time T1, there are rows in the `User` table (2 tuples in the `User` relation), however at time T2 more have been added (there are now 3 tuples in the `User` relation). `User` has a relation value but is a variable (relation variable).

  