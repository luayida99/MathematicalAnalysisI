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

Ex 2.2.1. Prove (a+b)+c = a+(b+c).  

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
