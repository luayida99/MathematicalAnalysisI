Integers: Starting with NxN space, place an equivalence relation ~ on (a,b)         
s.t. (a,b)~(c,d) <=> a+d = b+c. a--b = {(c,d) element of NxN:(a,b)~(c,d)}.        

Ex 4.1.1 Verify that equality on integers is an equivalence relation:         

Reflexivity:        
a+b = a+b <=> a--b = a--b         

Symmetry:       
a+d = b+c <=> a--b = c--d           
c+b = d+a <=> c--d = a--b           

Transitivity:         
a--b = c--d, c--d = e--f        
a+d = b+c, c+f = d+e
a+c+d+f = b+c+d+e         
a+f = b+e <=> a--b = e--f       

QED.              
