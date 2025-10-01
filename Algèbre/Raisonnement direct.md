## Définition

> [!hint] On résous une équation pour vérifier si l'implication (si P, alors Q) est ``Vraie``.

- On forme cet énoncé :
- Pour tout entier n, si n est pair, alors n² est pair
	- $\forall n \in \mathbb{N}, (\exists k \in \mathbb{N}, n = 2k) \implies (\exists l \in \mathbb{N}, n² = 2l)$

| Francais           | Algèbre                                         | Type               |
| ------------------ | ----------------------------------------------- | ------------------ |
| pour tout entier n | $\forall n \in \mathbb{N}$                      | Quantificateur     |
| n est pair*        | $\exists k \in \mathbb{N}, n = 2k$              | Hypothèse (si)     |
| n² est pair        | $\Rightarrow \exists l \in \mathbb{N}, n² = 2l$ | Conclusion (alors) |
- \*si $n = 2k$, alors le diviser par deux donne un entier k : $\frac{n}{2} = k$
	- c'est le moyen d'écrire que n est pair

> [!hint] On pourrais aussi écrire $\forall n \in \mathbb{N}, \exists k \in \mathbb{N},\exists l \in \mathbb{N}, (n = 2k \implies n² = 2l)$


___

> [!NOTE] Raisonnement pour savoir si n² est pair
> - $n² = 2k \times 2k = 4k²$
> - $n² = 2 (2k²)$
> - $n² = 2l$
> 	- avec $l = 2k²$
> - On a prouvé que si n est pair, n² est lui aussi pair


- On peux aussi résoudre ce problème avec le [[Raisonnement par Contraposée]]