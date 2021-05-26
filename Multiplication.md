Ex 2.3.1 Prove commutativity of multiplication.       

Induct on n, fixing m.      
Base case: n=0, 0 x m = 0 = m x 0       
Assume P(n) is true i.e. n x m = m x n      
To prove P(n+1) is true i.e. (n++) x m = m x (n++)        
LHS = (n x m) + m by Definition 2.3.1     
    = (m x n) + m by inductive hypothesis     
    = m x (n++)     
QED.      

Ex 2.3.2 Prove that positive natural numbers have no zero divisors.     

Let n,m be natural numbers. n x m = 0 <=> n = 0 or m = 0      

(=>):       
n x m = 0 = n x 0 = m x 0       
Therefore n = 0 or m = 0.       

(<=):       
n = 0, n x m = 0 x m = 0      
m = 0, n x m = n x 0 = 0      

QED.      

Prove distributivity of multiplication:       

Let a,b,c be natural numbers. a(b+c) = ab+ac, (b+c)a = ba+ca.       
Notice that the second identity follows from the proof of the first by        
commutativity.        

Induct on c, fixing a and b.      
Base case: c = 0, a(b+0) = ab = ab + a(0)     
Assume P(c) is true i.e. a(b+c) = ab+ac     
To prove P(c+1) is true i.e. a(b+c++) = ab+a(c++)       
LHS = a(b+c)+a      
    = ab+ac+a by inductive hypothesis     
    = ab+(ac+a)     
    = ab+a(c++)     

QED.      

Ex 2.3.3 Prove associativity of multiplication.     

Let a,b,c be natural numbers. (axb)xc = ax(bxc)       

Induct on c, fixing a and b.      
Base case: (axb)x0 = 0 = ax(bx0)      
Assume P(c) is true i.e. (axb)xc = ax(bxc)      
To prove P(c+1) is true i.e. (axb)xc++ = ax(bxc++)
LHS = (axb)xc++     
    = (axb)xc + (axb)     
    = ax(bxc) + (axb) by inductive hypothesis     
    = ax(bxc + b)     
    = ax(bxc++)     

QED.      

Prove that multiplication preserves order.      

Let a,b be natural numbers s.t. a < b, c is positive. Then ac < bc.     

By Definition 2.2.11, b = a+d for some positive d.              
Using that fact that multiplication is distributive, bc = ac+cd.      
Since d is positive, cd is positive. Therefore ac < bc.     

QED.      

Prove the cancellation law for multiplication.      

Let a,b,c be natural numbers s.t. ac = bc, c is nonzero. Then a=b.      

By Proposition 2.2.13, the trichotomy of order breaks the problem into 3 cases.       

Case 1:       
a < b.      
Using the fact that multiplication preserves order, ac < bc which is        
a contradiction.        
Case 2:
a > b.
Proof follows from case 1.      

Therefore, the only possibility is a=b.       

QED.        

Ex 2.3.4 Prove (a+b)^2 = a^2 + ab + b^2.      

Induct on a, fixing b.      
Base case: a=0, (0+b)^2 = b^2 = 0^2 + 0b + b^2            
Assume P(a) is true i.e. (a+b)^2 = a^2 + 2ab + b^2.        
To prove P(a+1) true i.e. (a++ +b)^2 = a++^2 + 2a++b + b^2.        
LHS = [(a+b)++]^2     
    = (a+b+1) x (a+b+1)       
    = (a+b)^2 + (a+b) + (a+b) + 1 x 1 by distributivity       
    = a^2 + 2ab + b^2 + 2(a+b) + 1 by inductive hypothesis      
    = (a^2 + 2a + 1) + 2b(a++) + b^2 by distributivity        
    = (a++)^2 + 2a++b + b^2       

QED.        

Ex 2.3.5 Prove the Euclidean Algorithm.       

Let n be a natural number, and let q be a positive number.      
Then there exists natural numbers m,r s.t. 0 <= r < q and n = mq+r.       

Induct on n, fixing q.      
Base case: n=0, 0 = 0q + 0        
Assume P(n) is true i.e. n = mq1 + r1       
To prove P(n+1) is true i.e. n++ = mq2 + r2       
LHS = n + 1       
    = mq1 + r1++ by inductive hypothesis        

Since 0 <= r1,r2 < q, 0 < r1++ <= q.      

Case 1: r1++ = q.     
LHS = m(q1++) + 0       
    = mq2 + r2, q2 = q1++, r2 = 0               

Case 2: r1++ < q.       
LHS = mq1 + r1++        
    = mq2 + r2, q1 = q2, r1++ = r2      

QED.        
