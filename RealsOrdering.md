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
