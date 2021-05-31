Ex 6.1.1 Given an (a sequence of real numbers) s.t. an+1 > an for each natural number n, prove that for natural 
numbers m and n where m > n, am > an.                       

Let inductive hypothesis be an+k > an for any natural number k.             
Base case: k=1, an+1 > an as given.                     
Inductive case: an+k > an => an+k+1 > an.                   
an+k+1 > an+k > an.                 
Then for any natural number m > n, we can rewrite m = n + l > n.                    
QED.                

Ex 6.1.2 Let an be a sequence of real numbers, and let L be a real number. Show than an(n>=m) converges to L <=> For any given real eps > 0                     
we can find an N >= m s.t. |an - L| <= eps for all n >= N.                          

(=>): Suppose an(n>=m) converges to L. This implies an is eventually eps-close to L i.e there exists a natural number N >= n s.t. an(n>=N) is eps-close to L. This is equivalent to |an - L| <= eps for some N >= n.            
(<=): Suppose |an - L| <= eps for all n >= N >= m. This implies we can find an N s.t. |aN - L| <= eps.             
By Definition 6.1.5, we have that an is eps-close to L for all n >= N. Since eps can be arbitrarily chosen, it    
follows that an converges to L.                 
QED.                    

Ex 6.1.3            
(=>): For some eps > 0, there exists N >= m s.t. |an - c| <= eps for all n >= N. Since m' >= m,                 
m' = m + k, k is a non-negative integer. Hence for all n >= m' |an - c| <= eps hence an converges to c.           
(<=): For some eps > 0, there exists an N >= m' s.t. |an - c| <= eps for all n >=  N.Then N >= m' >= m          
hence |an - c| <= eps for all n >= m and an converges to c.                 
QED.

Ex 6.1.4 
(=>): For some eps > 0, there exists N >= m s.t. |an - c| <= eps for all n >= N. n+k >= n >= N, thus            
|an+k - c| <= eps for all n >= N.               
(<=): For some eps > 0, there exists N >= m s.t. |an+k - c| <= eps for all n >= N. Choose N' = N + k <= n          
then N <= n - k.  Thus |an - c| <= eps and hence converges to c.                
QED.

Ex 6.1.5                
For some eps > 0, there exists N >= m s.t. |aj - L| <= eps/2 for all j >= N. Similarly there exists             
N' >= m s.t. |ak - L| <= eps/2 for all k >= N'. Then |aj - ak| <= |aj - L| + |ak - L| <= eps for all            
j,k >= max(N, N').                  
QED.

Ex 6.1.6            
Assume for sake of contradfiction an doesn't converge to L. Then for some eps > 0 there exists N >= m           
s.t. |an - L| > eps for all n >= N. Since an is Cauchy, the exists N' >= m s.t. |aj - ak| <= eps/2 for             
all j,k >= N'. Then there exists n0 >= N' s.t. |an0 - L| > eps, |an - an0| <= eps/2 for all n >= N'.            
Hence an0 - eps/2 <= an <= an0 + eps/2.                         

If an0 - L is nonnegative an0 - L > eps, an0 - eps/2 <= an for all n >= N'. Hence an > L + eps/2.           
By defining a new equivalent sequence bn s.t. bn > L + eps/2 we have L >= L + eps/2 which is a contradiction.      
If an0 - L is negative L - an0 > eps, an <= an0 + eps/2 for all n >= N'. Hence an < L - eps/2.              
Defining a new equivalent sequence then yields L <= L - eps/2 which is a contradiction.                 
QED.                    