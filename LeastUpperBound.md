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
