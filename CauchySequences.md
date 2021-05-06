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

Given that an and bn are equivalent sequences, prove that an is Cauchy sequence
<=> bn is Cauchy sequence.            

(=>): Let an and bn be equivalent sequences, epsilon>0 be given. Then             
|an-bn| < epsilon/3, for all n > N0 element of N. Assume an is a Cauchy sequence,           
then |am-an|< epsilon/3, for all m,n > N1 element of N.            
Then for any N = max(N0,N1),
|bm-bn| = |bm-am+am-an+an-bn|           
        <= |bm-am|+|bn-an|+|am-an|
        < epsilon
(<=): Symmetric argument.         

QED.             

Let epsilon>0. Show that if an and bn are eventually epsilon-close, an is           
bounded <=> bn is bounded.            

(=>): Let an and bn be epsilon-close sequences, epsilon>0 be given. Then          
|an-bn| < epsilon, for all n > N0 element of N. Assume an is bounded, hence            
|ai| < M for some M >= 0, 1 <= i element of N .           
|bi| = |bi-ai+ai| <= |ai-bi| + |ai| < epsilon + M           
Hence bn is epsilon+M bounded.          
(<=): Symmetric argument.           

QED.           
