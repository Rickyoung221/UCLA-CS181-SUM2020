<img src="/Users/rickyoung/Library/Application Support/typora-user-images/Screen Shot 2020-07-28 at 14.28.47.png" alt="Screen Shot 2020-07-28 at 14.28.47" style="zoom:130%;" />

<img src="/Users/rickyoung/Library/Application Support/typora-user-images/Screen Shot 2020-07-28 at 14.28.26.png" alt="Screen Shot 2020-07-28 at 14.28.19" style="zoom:130%;" />



**Decidable.** Proof:

Claim that if $L $ and $M$ both are context-free languages, then the language $L \cup M$ is context-free as well. (By Closure property under union). Proof for this:

Let $L = L(g), M = L(h).  $   $     g, h $ are CFG. 

Let $S(g) = S, S(h) = E$

Construct a new CFG $k$:

$S(k) = Q,$ 

add $Q \rightarrow S$, $Q\rightarrow E$ and all rules from $g$ and $h$ to $k$

$ \Rightarrow L(k) = L \cup M$

Therefore, $L\cup M$ is CFL. 

And clearly, $L \cup M ≠ \empty$ Iff at least one of them is not empty. In other words, $L \cup M$ is empty if both $L$ and $M$ are empty. 

Hence, to solve this problem, we need to test if any of $L$ and $M$ is empty . According to the lecture, we know that the problem of  “$L $ is CFL, is $L$ empty? “ is decidable. Clearly the problem in the lecture could be extended to the given problem in homework. i.e., the given problem could be solved by speartating into two problems of determine if a CFL $L$ is empty. If both are empty, then $L \cup M$ is empty; otherwise, it is not empty.

So there is a valid algorithm to solve the given problem, the answer could be yes or no.  Therefore, the problem is decidable. 

Proved.



<div style="page-break-after:always;"></div>



<img src="/Users/rickyoung/Library/Application Support/typora-user-images/Screen Shot 2020-07-28 at 14.28.37.png" alt="Screen Shot 2020-07-28 at 14.28.37" style="zoom:130%;" />



**Undecidable:**

Proof:

Similary like question 1, $(L \cap N) \cup (N\cap M)$ is empty iff both of $L \cap N$ and $N \cap M$ are empty.   

Support the problem is decidable. 

Support $M = \empty$, $M $ still is CFL. 

Then 

$(L \cap N) \cup (N\cap M)$

= $(L\cap N) \cup (N\cap \empty)$

= ($L \cap N) \cup \empty$ 

= $L \cap N$ 

From above,  “$L, N$ are CFL, does $L \cap N = \empty $” is decidable. 

However, as from the lecture, we know that the problem of “ $L, M$ are CFL, does $L \cap M≠\empty ?$ ” is undecidable. 

Contradiction!

Therefore, the given problem is undecidable. 

