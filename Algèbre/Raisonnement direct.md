## Définition

> [!hint] On résous une équation pour vérifier si l'implication (si P, alors Q) est ``Vraie``.

## Exemple
On forme cet énoncé :
- Pour tout entier n, si n est pair, alors n² est pair :
-  $\forall n \in \mathbb{N}, (\exists k \in \mathbb{N}, n = 2k) \implies (\exists l \in \mathbb{N}, n² = 2l)$
- C'est sous la forme $P \Rightarrow Q$
> [!hint] On pourrais aussi écrire $(\forall n \in \mathbb{N}, \exists k \in \mathbb{N},\exists l \in \mathbb{N}), (n = 2k \implies n² = 2l)$

| Francais                                                                   | Algèbre                                                                                      | Type                                            |
| -------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------- | ----------------------------------------------- |
| - pour tout entier n<br>- il existe un entier k<br>- il existe un entier l | - $\forall n \in \mathbb{N}$<br>- $\exists k \in \mathbb{N}$<br>- $\exists l \in \mathbb{N}$ | Quantificateurs :<br>Introduisent les variables |
| n est pair*                                                                | $n = 2k$                                                                                     | Hypothèse (si)                                  |
| n² est pair                                                                | $n² = 2l$                                                                                    | Conclusion (alors)                              |


___

> [!NOTE] Raisonnement pour savoir si n² est pair
> - $n² = 2k \times 2k = 4k²$
> - $n² = 2 (2k²)$
> - $n² = 2l$
> 	- avec $l = 2k²$
> - On a prouvé que si n est pair, n² est lui aussi pair


- On peux aussi résoudre ce problème avec le [[Raisonnement par Contraposée]]