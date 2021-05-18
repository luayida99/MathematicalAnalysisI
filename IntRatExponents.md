Ex 5.6.1 Prove Lemma 5.6.6.               

Let x,y >= 0 be non-negative reals, n,m >= 1 be positive integers.                      

(a) y = x^(1/n) => y^n = x:            
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

(b)y^n = x => y = x^(1/n):              
y^n = x => (y^n)^(1/n) = x^(1/n) = z => z^n = x. By Proposition 5.6.3 z = y.              

(c) x^(1/n) is a positive real number:            
For some non-negative real number x, 0 >= 0 and 0^n <= x => 0 element of              
{y element of R: y >= 0 and y^n <= x} => x^(1/n) is upper bound for this set.             
Hence x^(1/n) is non-negative. If x is positive, assume that x^(1/n) is not positive.                
But x^(1/n) must be 0 and hence not positive, which is a contradiction.               
Suppose x^(1/n) is positive, assume x is not positive. This implies x = 0.            
Hence x^(1/n) = 0^(1/n). Now consider the set E = {y element of R: y >= 0 and                     
y^n <= 0}. Then for any z > 0, z^n > 0 and thus not in the set. Hence supE = 0          
and hence x^(1/n) = 0^(1/n) = 0, which is a contradiction.            

QED.             

(d) x > y <=> x^(1/n) > y^(1/n):            
(=>): Suppose x > y => x^(1/n) <= y^(1/n). But 0 <= x^(1/n)n <= y^(1/n)n => x <= y                
by (a), which is a contradiction.           
(<=): Suppose x^(1/n) > y^(1/n), then x > y >= 0.                 

QED.              

(e) x > 1 => x^(1/k) decreasing function, x < 1 => x^(1/k) increasing function, x = 1                 
=> x^(1/k) = 1:               
Let a > b be 2 positive integers. If x > 1, suppose x^(1/a) >= x^(1/b). Then x^b >= x^a.                
Since a > b, a = b + r for some positive integer r. Hence x^b >= x^b x^r. Given x > 1,            
let inductive hypothesis be x^n > 1 for all positive integer n.             
Base case: x > 1              
Inductive case: x^(n+1) = x^n x > x > 1                 
Set n = r, we have x^r > 1 => x^b > x^b x^r which is a contradiction.                 
If x < 1, let c > d be 2 positive integers. Suppose x^(1/c) <= x^(1/d). Then x^d <= x^c.            
c = d + r => x^d >= x^d x^r, using the previous induction forms a contradiction.               
If x = 1, 1^k = 1 by (a) hence 1 = 1^(1/k).               

QED.                  

(f) (xy)^(1/n) = x^(1/n) y^(1/n):             
(xy)^(1/n)n = xy. (x^(1/n)y^(1/n))^n = (x^1/n)n (y^1/n)n = xy = (xy)^(1/n)n.              

QED.            

(g) (x^(1/n))^(1/m) = x^(1/nm):                   
((x^(1/n))^(1/m))^mn = (((x^(1/n))^(1/m))^m)^n = (x^(1/nm))^nm.             

QED.                        

Ex 5.6.2 Let x,y > 0 be positive reals, q,r be rationals.           

(a) x^q is a positive real:              
For integers a,b, q = a/b. x^q = (x^a)^(1/b) which is positive.           

(b) x^(q+r) = x^q x^r and (x^q)^r = x^(qr):               
q = a/b, r = c/d. x^(q+r) = x^((ad+bc)/bd) => x^((q+r)bd) = x^(ad+bc).            
(x^q x^r)^bd = (x^(a/b) x^(c/d))^bd = x^(abd/b) x^(bcd/d) = x^ad x^bc = x^(ad+bc).          
(x^q x^r)^bd = x^(q+r)^bd => x^(q+r) = x^q x^r.             

((x^q)^r)^bd = (x^(ac/bd))^bd = x^ac. (x^qr)^bd = (x^(ac/bd))^bd = x^ac.              
By cancellation law the result follows.             

(c) x^(-q) = 1/x^q:             
Let induction hypothesis be x^-n = 1/x^n for some integer n.              
Base case: x^0 = 1/x^0 = 1.             
Inductive case: x^-(n+1) = x^-1 (1/x^n) = 1/x (1/x^n) = 1/x^(n+1)             
q = a/b, x^((-a)/b) = (x^(-a))^(1/b) = (1/x^a)^(1/b) = (1/x^(a/b)) = 1/x^q                

(d) q > 0, x > y <=> x^q > y^q:             
(=>): q = a/b, x^a > y^a => (x^a)^(1/b) > (y^a)^(1/b) => x^q > y^q                 
(<=): q = a/b, (x^a)^(1/b) > (y^a)^(1/b) => x^a > y^a => x > y            

(e) x > 1 => x^q > x^r <=> q > r. x < 1 => x^q > x^r <=> q < r:             
q = a/b, r = c/d.             
If x > 1, we prove the following:             
(=>): q > r => ad > bc => ad-bc > 0. x > 1 => x^(1/k) > 1^(1/k) = 1 for some integer k.               
Let induction hypothesis be (x^(1/k))^n > 1.          
Base case: x^(1/k) > 1 as before.           
Inductive case: (x^(1/k))^(n+1) > x^(1/k) * 1 = x^(1/k) > 1.              
Hence x^(ad/bc) > 1 => x^ad > x^bc => x^(a/b) > x^(c/d) => x^q > x^r.                 
(<=): x^q > x^r => (x^a/b)^bd > (x^(c/d))^bd => x^ad > x^bc => x^(ad-bc) > 1.           
Suppose ad-bc <= 0, x^(ad-bc) = 1/x^(e) <= 1 which is a contradiction. Hence ad-bc > 0 =>                
ad > bc => a/b > c/d => q > r.                     
The x < 1 case is similar.                    

QED.            

Ex 5.6.3 x is real number => |x| = (x^2)^(1/2).               

x = 0: |0| = 0, (0^2)^(1/2) = 0.              
x > 0: |x| = x, (x^2)^(1/2) = x.            
x < 0: -x > 0, ((-x)^2)^(1/2) = -x. |x| = -x.           

QED.                                
