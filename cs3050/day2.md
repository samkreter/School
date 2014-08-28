//august 28 2014 

*Loop invariant*
initialization
Maintenance
Termination

*Random Access machine Model(RAM)*: An abstract (but realistic) model of computation.
+Single process model
+each basic intruction takes a constant amount of time. Three Kinds
	1)Arithmetic
	2)Data movement: Load, store, copy
	3)Control: conditional and unconditional branching, functions/procedure call and return
-person with a pen and paper

##Example with insertion sort
-Depeands on the number of elements int the sequence
+Take differnt amounts of time on two inputs of the same size
-Assuming that each pseudocode line has only primitive options, each line of scode reuqires a constant amount of time 
-differnet scode lines may take different times, but each execution of line i taks same ci

Average case analysis is often as bad as worst case analysis

*Order of growth:* Focuse on the most important determining facter
Insertion sort, T(n) = dn^2 + en + f. T(n) = Theta(n^2)

##Example with searching an array
Worst case is when the number is not in the array 
T(n) = 3n + 5 = Theta(n)

##Example with searching a sorted array(binary search)
Worst case is when the number is not in the array 
-all lines take 1 except 
-Every function call takes half the time becuase there are half as many elements in the array being searched
These are called recrrence equations
*Theta(og2n)*

##Big O
Asymptotic analysis - ignore all lower order functions 
