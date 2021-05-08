Prove that formal limits are well defined.        

x = x:
For all n >= 1, we have |an - an| = 0 < epsilon.                  

x = y => y = x:
For all n >= N, we have |an - bn| < epsilon. But |an - bn| = |bn - an|.             

x = y and y = z => x = z:         
For all n >= N1, we have |an - bn| < epsilon/2. For all m >= N2, we have          
|bn - cn| < epsilon/2. Then |an - cn| = |an - bn + bn -cn| <= |an - bn| +             
|bn - cn| < epsilon.          

QED.            

Prove that multiplication is well defined.          

x * y = xy:         
Let epsilon > 0 be given. By definition we have that |an - am| < epsilon1,            
|bl - bk| < epsilon2, n,m >= N1, l,k >= N2. Since x and y are Cauchy they are           
bounded by M1 and M2 respectively.          
Choose N = max(N1, N2),               
|anbn - ambm| = |anbn - anbm +anbm - ambm|          
              <= |an||bn - bm| + |bm||an - am|          
              = M1 * epsilon1 + M2 * epsilon2            
Choose epsilon1 = epsilon/2M1 and epsilon2 = epsilon/2M2, we have that            
|anbn - ambm| < epsilon. This implies that the sequence anbn is eventually          
epsilon-close as desired.               

x = x' => xy = x'y:             
Let epsilon > 0 be given. Since x = x' an and an' are eventually epsilon1-close             
i.e. |an - an'| < epsilon1 for some n >= N1. Notice that bn is Cauchy and hence           
bounded by some M. Choosing N = N1,                     
|anbn - an'bn| = |bn||an - an'|
               < M * epsilon1           
Choose epsilon1 = epsilon/M, it follows that anbn is eventually epsilon close               
to an'bn.           

QED.

Ex 5.3.4 For ratioanls a,b, prove that a=b <=> LIM(n -> INF)a = LIM(n -> INF) b.           

(=>): a = b => |a - b| = 0 < epsilon.         
(<=): Proof by contrapositive. Suppose a != b. Then for some n >= N1 there            
exists an epsilon s.t. |a - b| > epsilon > 0. Since a != b, |a - b|/2 > 0.          
Choose epsilon as |a - b|/2 then we have |a - b| > epsilon hence            
LIM(n -> INF)a = LIM(n -> INF)b.            

QED.          

Let an be a bounded sequence and bn be another sequence equivalent to an. Show              
bn is also bounded.             

Since an equivalent to bn, we have that an is eventually epsilon-close to bn.         
Choose epsilon = 1, by Exercise 5.2.2 bn is bounded.            

QED.          

Ex 5.3.5 Prove LIM(n -> INF) 1/n = 0.           

Let epsilon > 0 be given. By Proposition 4.4.1 there exists N > 1/epsilon.            
For some n >= N, n >= 1/epsilion > 0 => 0 < 1/n <= epsilon. Since |1/n - 0|             
= 1/n <= epsilon.             

QED.            

