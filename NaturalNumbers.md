Proof of additive commutativity:      

Claim: For any natural numbers n and m, n + m = m + n.      

Using induction on n (keeping m fixed).     
Base case: n = 0, 0+m = m = m+0 by Lemma 2.2.2 and definition of addition
on the natural numbers.
Assume P(k) is true i.e. k+m = m+k for any natural number k     
To prove P(k+1) true i.e.(k++)+m = m+(k++)      
LHS = (k++)+m     
    = (k+m)++ by definition of addition     
    = (m+k)++ by inductive hypothesis P(k)      
    = m+(k++) by Lemma 2.2.3 = RHS      

QED.

Proof of cancellation law:      

Claim: Let a,b,c be natural numbers s.t. a+b = a+c. Then b=c.     

Using induction on a (keeping b and c fixed).     
Base case: 0+b = 0+c, b=c by definition of addition.      
Assume P(n) is true i.e. n+b = n+c => b=c for any natural number n.
To prove P(n+1) true i.e. (n++)+b = (n++)+c => b=c.     
(n++)+b = (n+b)++     
(n++)+c = (n+c)++     
By Axiom 2.4, n+b = n+c.      
By inductive hypothesis, b=c.     

QED.

Proof of basic properties of ordering on the natural numbers:     
Let a,b,c be natural numbers.
     
(a) Order is reflexive, a >= a.

a = a+0 by Lemma 2.2.2      
  = a+m, m=0      
  >= a by Definition 2.2.11     

(b) Order is transitive, a >= b and b >= c => a >= c.     

By Definition 2.2.11, a = b+m1, b = c+m2, m1 and m2 are natural numbers.      
a = (c+m2)+m1     
  = c+(m2+m1) by associativity 
  = c+m3, m3=m2+m1      
Therefore a >= c by Definition 2.2.11.      

(c) Order is antisymmetric, a >= b and b >= a => a = b.     

By Definition 2.2.11, a = b+m1, b = a+m2, m1 and m2 are natural numbers.
a = (a+m2)+m1       
  = a+(m2+m1) by associativty      

By the cancellation law, m2+m1 = 0      
Using induction on a (keeping b fixed),      
let inductive hypothesis be a+b = 0 => b=0      
Base case: a=0, 0+b = b = 0 by Lemma 2.2.2      
Assume P(a) is true i.e. a+b = 0 => b=0
To prove P(a+1) true i.e. (a++)+b = 0 => b=0
LHS = (a++)+b     
    = (a+b)++ by definition of addition on natural numbers      
    = 0     
Since 0 is not a successor of any natural number, a+b = 0.      
By the inductive hypothesis, b=0.
Therefore m1=0.     
a = b+m1      
  = b+0     
  = b by Lemma 2.2.2      

(d) Addition preserves order, a >= b <=> a+c >= b+c     

(=>): By Definition 2.2.11, a = b+m1, m1 is a natural number.
a+c = (b+m1)+c      
    = (b+c)+m1 by associativity     
Therefore a+c >= b+c.     

(<=): By Definition 2.2.11, a+c = (b+c)+m1, m1 is a natural number.     
a+c = (b+m1)+c by associativity     
a = b+m1 by cancellation law.
a >= b by Definition 2.2.11

(e) a < b <=> a++ <= b      

(=>): By Definition 2.2.11, a <= b and a != b.      
a = b+m1, m1 is a natural number.     
a++ = (b+m1)++      
    = b+(m1)++
    = b+m2, m2 is a natural number      
Hence a++ <= b by Definition 2.2.11.      

(<=): Since a++ is the successor of a, a <= a++ and a != a++.     
Hence a < a++ by Definition 2.2.11.       
a < a++ <= b      
Hence a < b by transitivity of the < operator.      

(f) a < b <=> b = a+d for some positive number d.     

(=>): By Definition 2.2.11, a <= b and a != b.      
a = b+m1, m1 is a natural number.     
Since a != b, m1 != 0. By definition of positive, m1 is positive.       
Set m1 = d, a = b+d.               

(<=): Using b = a+d, b >= a by Definition 2.2.11.
Since d is a positive number, a+d != b by definition of positive.       
Since b >= a and b != a, a < b.       

Ex 2.2.1. Prove (a+b)+c = a+(b+c). (Associativity)     

Fix a and b as constants, do induction on c.  
Base case: c = 0, (a+b)+0 = a+b = a+(b+0)  
Assume P(c) is true i.e. (a+b)+c = a+(b+c)  
To prove P(c+1) true i.e. (a+b)+c++ = a+(b+c++)  
LHS = (a+b)+c++  
    = ((a+b)+c)++ by Lemma 2.2.3  
    = (a+(b+c))++ by inductive hypothesis P(c)  
    = a+(b+c)++ by Lemma 2.2.3  
    = a+(b+c++) by Lemma 2.2.3 = RHS

QED.

Ex 2.2.2 Let a be a positive number. Prove there exists exactly 1 natural number b s.t. b++ = a.    

<=> a = 0 or there exists 1 natural number b s.t. b++ = a.  
Base case: a = 1,  
0++ = 1 by definition (Proof of existence)  
Suppose there are 2 positive natural numbers c and d s.t. c++ = 1 and d++ = 1.  
By Lemma 2.2.6, c = d. (Proof of uniqueness)  

Assume P(a) is true i.e. There exists exactly 1 natural number d s.t. d++ = a.  
To prove P(a++) true i.e. There exists exactly 1 natural number d s.t d++ = a++.  
Let d = a. Then d++ = a++ by definition (Proof of existence)   
Suppose there are 2 positive natural numbers e and f s.t. e++ = a++ and f++ = a++.  
By transitivity, e++ = f++.
By Lemma 2.2.6, e = f (Proof of uniqueness)

QED.

Ex 2.2.4 Prove the trichotomy of order for natural numbers.       
Let a,b be natural numbers. Then exactly one of the following statements is         
true: a < b, a = b, a > b.      

Assume more than one statement is true. If a < b or a > b then a != b by definition.
If a > b and a < b, then a = b by Proposition 2.2.12 which is a contradiction.      
Hence no more than one statement is true.       

To prove at least one statement is true, induct on a and keep b fixed.      
Base case: a = 0, b >= 0 due to the fact that a and b are natural numbers, and      
0 has no successor.     
Assume P(a) true i.e. At least one statement is true for a, b.      
To prove P(a+1) true i.e. At least one statement is true for a++, b.      
Case 1: a < b, a++ <= b by Proposition 2.2.12.      
Case 2: a = b, a++ = b+m1 > b.      
Case 3: a > b, a++ > b.     
Therefore, inductive hypothesis is true.      

QED.        

Ex 2.2.5 Prove the Principle of Strong Mathematical Induction.      

Let Q(n) be the property that P(m) is true for all m0 <= m < n.      
Base case: Q(0) is vacuously true.      
Assume Q(n) true i.e. P(m) is true for all m0 <= m < n     
To prove Q(n+1) true i.e. P(m) is true for all m0 <= m < n+1       
By induction hypothesis P(n). Thus P(m) for all m0 <= m < n+1. Q(n+1) therefore       
is true.        

QED.      

Ex 2.2.6 Prove the Principle of Backwards Induction.        

Let induction hypothesis be (P(n) and (P(m++) => P(m))) => P(k) for any k <= n.       
Base case: n=1. P(1) and (P(m++) => P(m)). Specialising m++ to 1, m=0.      
Hence P(1) => P(0) so P(k) for any k <= 1.      
Assume P(n) is true i.e. (P(n) and (P(m++) => P(m))) => P(k) for any k <= n.
To prove P(n+1) is true i.e. (P(n+1) and (P(m++) => P(m))) => P(k) for any k <= n+1.
P(n+1) is true, P(n+1) => P(n). By induction hypothesis P(k) for any k <= n.      
Therefore P(k) for any k <= n+1.      

QED.        
