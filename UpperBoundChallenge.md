Let E be a nonempty subset of R. If E has an upper bound M, then it must have exactly 1 least upper bound.                          

Suppose E has more than 1 least upper bound, call them M1 and M2. M1>=M2 (M1 upper bound, M2 least upper)                   
and M2>=M1 (M2 upper bound, M1 least upper). Hence M1=M2 which is a contradiction.                                
It follows that E must have at most 1 least upper bound.            

Since E is nonempty, choose an element x from E. By the Archimedean property we have integers K, L s.t.         
K/n >= M and L/n < x. Since L/n < x and x is an element of E, L/n is not an upper bound for E. By Ex 5.5.2            
there exists an integer L < m <= K s.t. m/n is an upper bound for E but (m-1)/n is not. For any n,n'>=N,                         
where N is a positive integer, let m,m' be corresponding m. m/n > (m'-1)/n' => m/n - m'/n' > -1/n' >= -1/N.                     
By symmetry, m'/n' > (m-1)/n => m/n - m'/n' < 1/n <= 1/N. Hence |m/n - m'/n'| <= 1/N. By Ex 5.5.4 m/n is a            
Cauchy sequence. K = LIM(n -> INF)m/n = LIM(n -> INF)(m-1)/n. Since m/n is upper bound, x <= m/n =>             
x <= LIM(n -> INF)m/n = K, hence K is upper bound for E. For any upper bound M', M' >= (m-1)/n =>                                 
M' >= LIM(n -> INF)(m-1)/n = K. Since M' >= K, it follows that K is least upper bound for E. Hence E must have              
at least 1 least upper bound.             

Since E has at most and at least 1 least upper bound, the claim follows.            

QED.            
