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