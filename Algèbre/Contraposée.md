## Définition
- Dans une implication, pour trouver si l'assertion est vraie, au lieu de faire un [[Raisonnement direct]] on regarde si la contraposée est vraie
- si $non P \Rightarrow non Q$ est vrai, alors $P \Rightarrow Q$

> [!hint] Ces propositions sont équivalentes dans le sens ou prouver que l'une est vrai, prouve que l'autre est vraie

___
## Démonstration

> [!note] Enoncé
> - Pour tout entier n, si n est pair, alors n² est pair
>- On peux l'écrire sous forme algébrique :
>- $\forall n \in \mathbb{N}, (\exists k \in \mathbb{N}, n=2k) \Rightarrow (\exists l \in \mathbb{N}, n²=2l)$

> [!NOTE] Contraposée
>- Si n est impaire, n² est impaire
>- $\forall n \in \mathbb{N}, (\exists k \in \mathbb{N}, n=2k+1) \Rightarrow (\exists l \in \mathbb{N}, n²=2l+1)$ 
>- $n² = 2k+1$
>- $=4k²+4k+1$
>- $=2(2k²+2k) + 1$
>- $n² = 2l + 1$ avec $l = 2k²+2k$
>- Si n est impaire $(n=2k+1)$ on voit que n² est impaire $(n²=2l+1)$

- On à vérifié que la contraposée était Vraie, donc l'énoncé de base est Vrai