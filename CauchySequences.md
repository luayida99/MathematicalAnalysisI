Prove that every finite Cauchy sequence is bounded.          

Consider the finite sequence a1,...,an.           
Prove by induction on n.          
Base case: n=1, Sequence is bounded by |a1|.          
Assume P(n) is true i.e. a1,...,an is bounded.        
To prove P(n+1) is true i.e. a1,...,an,an+1 is bounded.         
By the induction hypothesis, a1,...,an is bounded by some M>=0.       
By definition of boundedness, it follows that a1,...,an+1 is bounded by           
M+|an+1|. Since |an+1|>=0, a1,...,an is also bounded by M+|an+1|.         

QED.          

Prove that every Cauchy sequence is bounded.          

By definition of Cauchy sequence, there always exists an n element of N s.t.            
an+1,... is epsilon-steady (any choice of epsilon>0 suffices). Now consider           
a1,...,an. Notice that it is bounded by the maximal element |ar|, r element of
N.              
Since any Cauchy sequence can be separated into a finite sequence and epsilon-          
steady sequence, and both these sequences are bounded by max(|ar|, epsilon),            
the claim follows easily.           

QED.            
