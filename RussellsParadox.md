Ex 3.2.1 Show that universal specification axiom implies Axioms
3.2,3.3,3.4,3.5,3.6.          

Axiom 3.2 Existence of empty set:       
From axiom of universal specification, y element of {x:P(x) true} <=> P(y)
true.         
Set P(x) as x != x, y element of {x:x != x} <=> y != y.         
But there exists no such y s.t. y != y, hence {x:x != x} is an empty set.         

Axiom 3.3 Singleton and pair sets:        
y element of {x:x = a} <=> y = a.         

Axiom 3.4 Pairwise Union:         
y element of {x: x element of A or B} <=> y element of A or B.          

Axiom 3.5 Specification:
y element of {x: x element of A and P(x)} <=> y element of A and P(y).        

Axiom 3.6 Replacement:          
z element of {y: P(x,y) for some x element of A} <=> P(x,z) for some x.           

QED.          

Ex 3.2.2 Show that if A is a set, A is not an element of A. Further, show that             
if A and B are sets, either A not element of B or B not element of A.         

Suppose there exists a set A s.t. A element of A and A element of {A}.          
Then A cannot be empty, since empty set has no elements.        
A n {A} = {x:x element of A and {A}}           
        = {x:x element of A and A} by definition of singleton set          
        = A           
By the regularity axiom, A n {A} = empty since the element in {A} is either not           
a set or disjoint from A.                   
This implies that A is empty, which is a contradiction.           

QED.          

Suppose A element of B and B element of A.        
Consider a set X = {A, B}. X is non-empty by definition.        
Further, notice that A and B must have non-empty intersection with X.         
This is a contradiction, which implies either X is not a set (impossible) or          
that either A not element of B or B not element of A.         

QED.          
