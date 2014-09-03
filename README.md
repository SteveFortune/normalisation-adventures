#Normalisation

This is a personal project documenting examples of database schemas in different normal forms. It is purely for my own interest and personal development so that I can become more proficient in designing scalable, transaction-oriented systems. 

I have also read various arguments for and against normalisation and would like to perform tests to determine which levels of normalisation suit different requirements. I'm aiming for this project to also be a personal reference point to decide when and how to structure my data.

###Objectives and Requirements

####Normalisation to 6NF

First I want to cover all the normal forms:

- 1NF schema & performance benchmarks by Oct 2014
- 2NF schema & performance benchmarks by Oct 2014
- 3NF schema & performance benchmarks by Oct 2014
- BCNF schema & performance benchmarks by Oct 2014
- 4NF schema & performance benchmarks by Nov 2014
- 5NF schema & performance benchmarks by Nov 2014
- 6NF schema & performance benchmarks by Dec 2014

####Denormalised and 'Un-normalised' Comparison

Then I want to compare benchmarks from the normal forms to benchmarks from schemas that are not normalised

- Denormalised schema & performance benchmarks by Dec 2014. Schema should be taken from 5NF into a selectively denormalised schema.
- 'Un-normalised' schema & performance benchmarks by Dec 2014. Schema should be designed from the ground up to be normalised pragmatically but without specific normalisation constraints in place.

####Benchmarks

Benchmarks should measure:

- Speed of various queries
- DB load testing
- Reports on the amount of anomylous and redundant data there is in the database

###Stack

- I have not decided what kind of stack I will be using yet for these examples.
- I'm probably going to look at using a mixture of different technologies for the different objectives here. As I use Doctrine allot in practice, I am aiming to use it as an ORM for as many of the schemas as possible.