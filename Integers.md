Integers: Starting with NxN space, place an equivalence relation ~ on (a,b)         
s.t. (a,b) ~ (c,d) <=> a+d = b+c. a--b = {(c,d) element of NxN:(a,b)~(c,d)}.        

Ex 4.2.1 Verify that equality on integers is an equivalence relation:         

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

Ex 4.2.2 Prove Lemma 4.2.3.         

Suppose a//b = a'//b'.          

Addition:           
a//b + c//d = a'//b' + c//d         
(ad+bc)b'd = (a'd+b'c)bd        
ab'd^2 + bcb'd = a'bd^2 + bcb'd which holds since ab' = a'b.            
Same holds for c'//d'.        

Multiplication:         
a//b x c//d = a'//b' x c//d       
ab'cd = a'bcd which holds since ab' = a'b.          
Same holds for c'//d'.          

Negation:         
-(a//b) = -(a'//b')           
-ab' = -a'b which holds since ab' = a'b.          
Same holds for c//d, c'//d'.            

QED.            

Ex 4.2.3 Prove the laws of algebra for rationals.         

Let x = a//b, y = c//d, z = e//f.         

x+y = y+x:        
x+y = a//b + c//d = (ad+bc)//bd         
y+x = c//d + a//b = (bc+ad)//bd           

(x+y)+z = x+(y+z):            
(x+y)+z = (ad+bc)//bd + e//f = (adf+bcf+ebd)//bdf             
x+(y+z) = a//b + (cf+de)//df = (adf+bcf+ebd)//bdf           

x+0 = 0+x = x:          
x+0 = a//b + 0//g = ag//bg = a//b = x           
x+0 = 0+x by 1st proposition.         

x+(-x) = (-x)+x = 0:        
x+(-x) = a//b + (-a)//b = (a-a)//b = 0//b = 0           
x+(-x) = (-x)+x by 1st proposition.           

xy = yx:          
xy = a//b x c//d = (ad+bc)//bd = c//d x a//b = yx           

(xy)z = x(yz):          
(xy)z = (a//b x c//d) x e//f = ac//bd x e//f = ace//bdf             
x(yz) = a//b x (c//d x e//f) = a//b x ce//df = ace//bdf           

x1 = 1x = x:          
x1 = a//b x 1//1 = a//b = x         
x1 = 1x by 5th proposition.         

x(y+z) = xy+xz:         
x(y+z) = a//b x (c//d + e//f)                 
       = a//b x (cf+de)//df               
       = (acf+ade)//bdf           
xy+xz = a//b x c//d + a//b x e//f           
      = ac//bd + ae//bf           
      = (acf+ade)//bdf            

(y+z)x = yx+zx:           
Follows from propositions 5, 8.           

QED.            

Ex 4.2.4 Prove the trichotomy of rationals.         

Assume more than 1 relation holds true. If x is positive or negative then it is             
nonzero by definition. If x is positive and negative then we reach
a contradiction.          
Hence at most 1 relation holds true.          

Let x be a rational number a/b, where a and b are integers.         
Notice that any permutation of cases for a and b (by the trichotomy on
integers)               
will result in the definition of either positive or negative rational or 0 or
undefined.            
Hence at least 1 relation holds true.           

QED.              
