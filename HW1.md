![](/Users/rickyoung/Library/Application Support/typora-user-images/image-20200702222659195.png)

**True**

Proof: (note that & means and, | means or)

1. (=>):

Suppose  $ \forall x,$  $x \in A\setminus(B \setminus C)$	

$x \in A\setminus(B \setminus C) $

$\Rightarrow$ $x \in A $ & $ x \notin (B \setminus C ) $

$\Rightarrow $ $ x \in A$ & $ \neg (x \in B\setminus C)$

$\Rightarrow$ $ x \in A $ & $\neg (x \in B$ & $x \notin C)$ 

By De Morgan’s Laws,

$\Rightarrow x \in A$ & $ (x \notin B$ | $x \in C)$

Case 1:

  $x \in A$ & $ x \notin B$ $\Rightarrow $ $ A \setminus B$

Case 2:

$x \in A$ & $x \in C$ $ \Rightarrow $ $ A \cap  C$

by above steps, 

$ \Rightarrow x \in (A \setminus B) \cup (A \cap C)$  , 

therefore, we can conclude that

$A\setminus(B \setminus C)$ $ \subseteq (A \setminus B) \cup (A \cap C) $



2. $(\Leftarrow)$:

Suppose $\forall z$, $ z \in $ $$ (A \setminus B) \cup (A \cap C) $$

$ z \in $ $$ (A \setminus B) \cup (A \cap C) $$

Case 1:

$ z \in (A \setminus B) $ $\Rightarrow$ $z \in A$ & $ z \notin B$

Case 2:

 $ z \in (A \cap C)$ $\Rightarrow $ $ z \in A$ & $ z \in C$

By above cases, 

$\Rightarrow$ $ z \in A$ & $ ( z \notin B$ |$ z \in C)$

Apply De Morgan’s law,

$\Rightarrow$ $ z \in A$ & $ \neg (z \in B$ & $ z \notin C)$

$\Rightarrow$ $z \in A$ & $ \neg (z \in (B \setminus C) )$

$\Rightarrow$ $ z \in A$ & $ z \notin (B \setminus C) $

$\Rightarrow $ $ z \in A\setminus(B \setminus C)$

So we can conclude that 

$(A \setminus B) \cup (A \cap C) $ $ \subseteq A\setminus(B \setminus C) $

Consequently, $A\setminus(B \setminus C)$ $ = (A \setminus B) \cup (A \cap C) $

**Proved. **

---

Also, use Venn diagram to verify the identity:

<img src="/Users/rickyoung/Library/Application Support/typora-user-images/image-20200703230652985.png" alt="image-20200703230652985" style="zoom:33%;" />



This can be verified easily from above diagram that $A\setminus(B \setminus C)$ $ = (A \setminus B) \cup (A \cap C) $.

