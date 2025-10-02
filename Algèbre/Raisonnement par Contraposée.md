## Définition
- Dans une implication, pour trouver si l'assertion est vraie, au lieu de faire un [[Raisonnement direct]] (vérifier $P \Rightarrow Q$) on regarde si la contraposée est vraie
- Si $(non P \Rightarrow non Q)$ est ``Vraie``, alors $(P \Rightarrow Q)$ est ``Vraie``

> [!hint] Ces propositions sont ``équivalentes``, dans le sens où prouver que si l'une est ``Vraie``, prouve que l'autre est ``Vraie``.

___
## Démonstration

> [!note] Enoncé
> - Pour tout entier n, si n est pair, alors n² est pair
>- On peux l'écrire sous forme algébrique :
>- $\forall n \in \mathbb{N}, (\exists k \in \mathbb{N}, n=2k) \Rightarrow (\exists l \in \mathbb{N}, n²=2l)$
>- Ici on as la forme $P \Rightarrow Q$

> [!NOTE] Contraposée de l'enoncé
>- Si n est impaire, n² est impaire
>- $\forall n \in \mathbb{N}, (\exists k \in \mathbb{N}, n=2k+1) \Rightarrow (\exists l \in \mathbb{N}, n²=2l+1)$ 
>- Ici on as la forme $non P \Rightarrow nonQ$
>- $n² = (2k+1)²$
>- $=4k²+4k+1$
>- $=2(2k²+2k) + 1$
>- $n² = 2l + 1$ 
>	- avec $l = 2k²+2k$
>- Si n est impaire $(n=2k+1)$ on voit que n² est impaire $(n²=2l+1)$

