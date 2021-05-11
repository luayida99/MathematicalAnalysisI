Prove that there exists a positive real x s.t. x^2 = 2.             

Let E = {y element R: y>=0 and y^2 < 2}. Notice E is upper bounded by 2 as 2^2 > 4 not element of E.                            
Also E is nonempty as 1 is element of E. By the least upper bound property (previously proven), there exists                    
a real number x=supE. Suppose x^2 < 2, then for some 0 < eps < 1, (x+eps)^2 = x^2 + 2eps x + eps^2                                 
<= x^2 + 4eps + eps = x^2 + 5eps, eps^2 <= eps and x <= 2. Thus we can choose eps s.t. x^2+5eps < 2. From this,                  
x^2+5eps < (x+eps)^2 < 2 and hence x+eps is an element of E. This is a contradiction as x+eps > x but x=supE.                     
Now suppose x^2 > 2, then for some 0 < eps < 1, (x-eps)^2 = x^2 - 2eps x + eps^2 >= x^2 - 4eps, eps^2 <= eps              
and x <= 2. Hence we can choose eps s.t. x^2-4eps > (x-eps)^2 > 2. Thus x-eps is greater than any element of E,                       
making it an upper bound for E. But this is a contradiction as x-eps < x but x = supE.                                        

QED.                              

Ex 5.5.1 Let E be a subset of R, suppose E has M=supE. Let -E = {-x:x element E}. Show -M = inf(-E).              

For some y element -E, we have y = -x where x is an element of E. x <= M => -x >= -M => y >= -M, hence -M is a lower                      
bound for -E. Consider any lower bound of -E and let it be L. L <= y => L <= -x => x <= -L, hence -L is an upper bound              
for E. But since M=supE, M <= -L => L <= M, and it follows that -M = inf(-E).                 

QED.              

Ex 5.5.2 Let E be nonempty subset of R. Let n,L,K be integers, n>=1, L < K, K/n is upper bound for E, L/n is not.                          
Show there exists an integer L < m <= K s.t. m/n is upper bound for E but (m-1)/n is not.                   

Suppose there is no integer L < m <= K s.t. m/n is upper bound but (m-1)/n is not.              
Let induction hypothesis P(k) be (K-k)/n is upper bound for E, k >= 0.              
Base case: K/n is upper bound for E.                       
Inductive case: (K-j)/n is upper bound for E, hence for any element x in E x <= (K-j)/n => L < K-j <= K.              
Suppose (K-j+1)/n is not an upper bound for E. But setting m = K-j would lead to a contradiction, hence the claim follows.                   
L < K => K-L > 0 hence (K-(K-L))/n = L/n is an upper bound for E which is a contradiction.                                            

QED.                         
