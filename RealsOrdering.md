Ex 5.4.1 Prove Proposition 5.4.4.            

Suppose more than 1 case is true.             
        
x is positive and 0:          
x = LIM(n -> INF)an, an >= c > 0 for all n         
|an - 0| = |an| >= c > c/2 which implies an is not c/2 close to 0.            

x is negative and 0:          
x = LIM(n -> INF)bn, -c <= bn, c > 0 for all n            
|bn - 0| = |bn| >= c > c/2 which implies bn is not c/2 close to 0.          

x is positive and negative:           
x = LIM(n -> INF)an, an >= c > 0 for all n         
x = LIM(n -> INF)bn, -d <= bn, d > 0 for all n            
|an - bn| >= c + d > (c + d)/2 which implies that an is not (c+d)/2 close to bn.             

Hence at most 1 claim is true.            

To prove that at least 1 claim must be true, consider x = 0 and x != 0.           
If x = 0 then the claim that x is 0 is true.          
If x != 0, then x = LIM(n -> INF)an for some Cauchy sequence an bounded away from 0.          
Since an is Cauchy, it is eventually epsilon1-steady for some n>=N.             
For some c > 0, |an| >= c. For all k >= N |ak - aN| < epsilon1.           

If aN > 0, |ak - aN| < epsilon1 => aN - ak < epsilon1 => aN - epsilon1 < ak             
Choose epsilon1 = c/2, 0 < c/2 < aN - c/2 < ak. Hence for all k >= N an is positively bounded.      
For all j < N set an = c/2, notice that this new sequence is eventually c/2 steady and equivalent to an.          
Then the new sequence is positively bounded implying that it is a positive real number.                                        

If aN < 0, |ak - aN| < epsilon1 => ak - aN < epsilon1 => -c <= ak < aN + epsilon1               
Choose epsilon1 = -c/2, -c <= ak < aN + epsilon1 < -c/2. Hence for all k >= N an is negatively bounded.           
For all j < N set an = c/2, notice that this sequence is eventually -c/2 steady and equivalent to an.       
Then the new sequence is negatively bounded implying that it is a negative real number.                                     

Hence at least 1 claim is true.           

Since at least and at most 1 claim is true, it follows that only 1 claim can be true.     

QED.                                       

Ex 5.4.2 Prove Proposition 5.4.7.               

Consider 3 real numbers x,y,z.              

(a) Trichotomy of order:          
Consider the real number x-y. By Proposition 5.4.4, x-y is either zero, positive or negative.
x-y = 0 => x = y              
x-y < 0 => x < y            
x-y > 0 => x > y              
Hence at least 1 claim is true.               
Assume more than 1 claim is true, then a similar breakdown of cases shows there always is a contradiction.          

(b) x < y <=> y > x:                                                                      
(=>): x < y => x-y < 0 => y-x > 0 (Proposition 5.4.4) => y > x           
(<=): y > x => y-x > 0 => x-y < 0 (Proposition 5.4.4) => x < y                  

(c) x < y and y < z => x < z:                 
x-y < 0 and y-z < 0 => (x-y)+(y-z) < 0 => x-z < 0 => x < z                  

(d) x < y => x+z < y+z:               
x-y < 0 => (x+z)-(y+z) < 0 => x+z < y+z                 

(e) x < y and z is positive => xz < yz:             
y-x > 0 => (y-x)z > 0 => xz < yz                

QED.              

Ex 5.4.3 Show that for every real number x there is exactly 1 integer N s.t. N <= x < N + 1.                    

Notice that x = LIM(n -> INF)an where an is a Cauchy sequence. Hence for all j >= N, |aj - aN| < epsilon1.              
-epsilon1 < aj - aN < epsilon1 => aN + epsilon1 < aj < aN + epsilon1 by Proposition 4.3.3.                                  
Choose epsilon1 = 1/2 and set an = aN for all n < N, then it follows that this sequence is equivalent and     
Cauchy. By Corollory 5.4.10 it follows that aN - 1/2 <= x <= aN + 1/2.                                           
By Proposition 4.4.1, we can find a M s.t. M <= aN < M+1.             
M - 1 <= aN - 1 < aN - 1/2 <= x < M + 1 + 1/2 < M + 2 => M - 1 < x < M + 2                
Order trichotomy then guarantees the existence of an integer satisfying the inequality.             
x < M => M - 1 <= x < M               
x >= M, x < M + 1 => M <= x < M + 1, x >= M + 1 => M + 1 <= x < M + 2                 
This proves the existence of an integer s.t. N <= x < N + 1.                

Now suppose that N is not unique. Then there exist n, m s.t. n <= x < n+1 and m <= x < m+1, n != m.               
n < m => n < m <= x < m+1. By definition of order we have m = n+d, n+1 = m+d' for positive integers d,d'.                 
n+1 = n+d+d' => d+d' = 1 which is a contradiction since d,d' are positive integers.                       
The n > m case is identical, and can be proven by n = m, m = n.                  
This completes the proof of uniqueness of N.                

QED.                                             
