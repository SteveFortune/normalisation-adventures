#2NF

- Relvar _R_ is in the second normal form if for every key _K_ of _R_ and every nonprime attribute _A_ of _R_, the FD _K → {A}_ is irreducible.

- Another way of looking at is, it: relvar _R_ is in the second normal form if for _X → Y_ one of the following is true:

	1. _X_ is a superkey
	
	2. _Y_ is a subkey
	
	3. _X_ is not a subkey
	
	
- I.e., subkeys can't hold FDs to nonprime attributes.

- Example


		VAR user BASE RELATION
			{ first_name CHAR, last_name CHAR, dob DATE, first_initial CHAR }
			KEY { first_name, last_name }
			
	- The following FD holds: `{ first_name, last_name } → { first_initial }` - the first initial is represents the first letter of the user's first name
	
	- This is _not_ in 2NF because a proper subkey holds an FD to a non-prime attribute. The FD above is not irreducible, it can be reduced to `{ first_name } → { first_initial }`