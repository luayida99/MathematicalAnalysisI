Ex 5.6.1 Prove Lemma 5.6.6.               

Let x,y >= 0 be non-negative reals, n,m >= 1 be positive integers.                      

(a) y = x^(1/n) => y^n = x            
Suppose y^n < x.           
Claim: (x+eps)^n <= x^n + M * eps for integers n.             
Base case: (x+eps)^1 <= x^1 + 1 * eps.            
Inductive case: (x+eps)^(n+1) <= (x+eps)(x^n + M * eps)               
                              = x^(n+1) + (M+1)eps * x^n + M * eps^2                
                              = x^(n+1) + [(M+1)x^n + M * eps] * eps                
Hence for some 0 < eps < 1, y^n + M * eps < x => (y+eps)^n < x. This implies that               
y+eps is an element of the set {z is real number: z^n <= x}. But this is a            
contradiction as y = x^(1/n) is an upper bound for the set.                 
The proof for y^n > x is similar, hence by trichotomy of equality on reals the                
result follows.                               

QED.              
