Ex 3.1.1 Show that Definition 3.1.4 is reflexive, symmetric, transitive.      

For sets A and B, A = B <=> For all x (x is element of A <=> x is element of B)       

Reflexivity:        
Since x is element of A <=> x is element of A, A = A.       

Symmetric:        
Since x is element of B <=> x is element of A, B = A.       

Transitive:       
Consider 3 sets A, B, C. x is element of A <=> x is element of B <=> x is
element of C.       

QED.        

Ex 3.1.2 Prove that empty, {empty}, {{empty}}, {empty, {empty}} are distinct.             

Recall that 2 sets A and B are distinct iff A != B.       
By Axiom 3.2, empty set contains no elements. Hence it is distinct from the
others, as they are nonempty sets.         
By Definition 3.1.4, {empty} is distinct as there is no other set that only
contains empty.         
By Axiom 3.1, {empty} is considered an object. By Definition 3.1.4 and Axiom
3.3, we then have that it is distinct since it is the only singleton set containing {empty}.            
By Axiom 3.3, {empty, {empty}} is a pair set of empty and {empty}. This is
distinct by Definition 3.1.4.       

QED.        

Ex 3.1.3 Prove that the union operation is commutative, associative and
A u A = A u empty = empty u A = A.        

Associativity:          
Consider 3 sets A, B, C.        
For associativity to hold, (A u B) u C = A u (B u C).         
Suppose x is an element of (A u B) u C. By Axiom 3.4, x is either an element of
A u B or C.         
Case 1:       
If x is element of A u B, then x is either element of A or B.         
If x is element of A, then it is element of A u (B u C) by Axiom 3.4.       
If x is element of B, then it is element of B u C by Axiom 3.4.         
It then follows that x is element of A u (B u C) by Axiom 3.4.        

Case 2:           
If x is element of C, then it is element of B u C by Axiom 3.4.       
By Axiom 3.4, x is element of A u (B u C).        

This implies that every element x in (A u B) u C is in A u (B u C).         
Using an identical argument successively applying Axiom 3.4, the reverse claim
is also trivially true.      
         
Therefore the union operation is associative.         

QED.          

Commutativity:          
Consider 2 sets A, B.       
For commutativity to hold, A u B = B u A.       
Suppose x is an element of A u B. By Axiom 3.4, x is either an element of A or
B.          
If x is element of A, it is element of B u A by Axiom 3.4.        
If x is element of B, it is also element of B u A by Axiom 3.4.         
This implies that every elemnt in A u B is in B u A.        
Using an identical argument, the reverse claim is also trivially true.        

Therefore the union operation is commutative.       

QED.        

A u A = A u empty = empty u A = A:          
Suppose x is an element of A.         
By Axiom 3.4, x is element of A u A.        
By Axiom 3.4, x is element of A u empty.        
This implies that every element in A is in A u A and A u empty.       

Suppose y is an element of A u A.       
By Axiom 3.4, y is either an element of A or A. Hence y is an element of A.       
An identical argument can be made for A u empty.        

By Definition 3.1.4, A = A u A = A u empty.         
By transitivity of the union operation, A u empty = empty u A.        
By associativity of =, the claim follows.       

QED.

Ex 3.1.5 Let A, B be sets. Show that A subset B, A u B = B, A n B = A are
logically equivalent.       

A subset B => A u B = B:        
By Definition 3.1.15, for any x, x element A => x element B.      
Hence every element in A is also in B.        
Suppose x is an element of B.       
By Axiom 3.4, x is element of B u A and hence A u B (by associativity of u).                
Suppose x is an element of A u B. By Axiom 3.4, x is either element of A or B.      
If x is element of B, argument is the same as above.      
if x is element of A, since every element of A is in B, x is in B.        

A u B = B => A n B = A:
Suppose there exists a x s.t. it is element of A but not element of A n B.        
Then x must be in A but not in B. But this is a contradiction as the existence        
of such a x must imply that A u B != B.         

A n B = A => A subset B:        
Suppose x is an element of A n B. By Definition 3.1.23, x is element of A and
B.          
By definition of set equality, all elements in A n B are in A and vice versa.       
If x is in A, then it must be in B as well from A n B = A. Thus for any object          
y, y is element of A => y is element of B, which is the definition of subset.       

QED.        

Ex 3.1.6 Prove Proposition 3.1.28.        
Let A, B, C be sets, X be set where A B C are subsets.        
(a) Minimal element       
By definition of union, A u empty implies that any object x is either        
an element of A or the empty set. Since empty set has no elements, any object x       
must belong in A.       

By definition of intersection, A n empty implies that any object x is in both       
A and the empty set. Since empty set has no elements, any object x must belong          
in A.               

(b) Maximal element         
A u X = X follows from definition of union, and A subset X.       
A n X = A follows from definition of intersection, and A subset X.        

(c) Identity      
A n A implies that any object x belonging to it is either in A or A. Hence any x is in         
A.        
A u A implies that any object x belonging to it is in both A and A. Hence any         
x is in A.          

(d) Commutativity         
Above.        

(e) Associativity       
Above.        

(f) Distributivity        
Consider any object x belonging to A n (B u C).        
A n (B u C) => x in both A and (B u C)        
x in (B u C) => x is B or C       
Hence x in both A and (B or C) => x in (A and B) or (A and C)       
=> A n (B u C) subset (A n B) u (A n C)        
Similar argument can be made for reverse claim.         

Consider any object x belonging to A u (B n C).         
A u (B n C) => x in A or (B n C)        
x in (B n C) => x in both B and C       
Hence x in A or (B and C) => x in (A or B) and (A or C)       
=> A u (B n C) subset (A u B) n (A u C)          
Similar argument can be made for reverse claim.         

(g) Partition           
Consider object x in A u (X\A).         
x in A or X\A => x in A or in X without A => x always in X as A subset X        
Reverse claim is trivially true.        

Consider object x in A n (X\A).         
x in A and X\A => x in A and not in A => empty set        
Reverse claim is trivially true.        

(h) De Morgan's Laws        
Consider an object x in X \ (A u B).        
x is in X but not in either A or B. This implies that x must be in both       
X\A and X\B. Hence X \ (A u B) subset (X\A) n (X\B).         
The reverse claim uses the same reasoning.        

Consider an object x in X \ (A n B).          
x is in X but not in both A and B. This implies that x must be in either X\A          
or X\B. Hence X\ (A n B) subset (X\A) u (X\B).        
The reverse claim uses the same reasoning.        

Ex 3.1.11 Show that the axiom of replacement implies axiom of specification.         
The axiom of replacement states that z is an element of {y: Q(x,y) true for         
some x element of A} <=> Q(x,z) is true for some x element of A.        

Choose Q(x,y) = y and P(x). Applying the axiom of replacement yields        
{y: Q(x,y) is true for some x element of A} = {x element of A: x = x and P(x)}        
which is equivalently {x element of A: P(x) is true}, the axiom of
specification.        
