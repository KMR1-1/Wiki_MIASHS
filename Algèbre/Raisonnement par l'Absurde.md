## Définition

> [!NOTE] On as une implication $P \Rightarrow Q$
> - On va nier l'implication ce qui donne $P \Rightarrow nonQ$
> - Ensuite on va chercher à trouver une contradiction dans cette nouvelle implication
> - Cette contradiction prouve que $P \Rightarrow Q$ est ``Vraie``

## Exemple

> [!example] Prouver que si $\frac{a}{1+b} = \frac{b}{1+a}$ alors $a=b$
> - $(\forall a,b \in \mathbb{N}), (a,b \geq 0), (\frac{a}{1+b} = \frac{b}{1+a}\Rightarrow a=b)$
> - Pour nier cet énoncé, on suppose que $a \neq b$ et on cherche un contradiction à ça
> $$\frac{a}{1+b} = \frac{b}{1+a}$$
> - On fait un produit en croix
> $$\frac{a(1+a)}{(1+b)(1+a)} - \frac{b(1+b)}{(1+a)(1+b)} = 0$$
>  $$\frac{a(1+a) - b(1+b)}{\cancel{(1+b)(1+a)}} = 0$$
>  - On peux retirer le diviseur :
> $$a(a+1) - b(b+1) = 0$$
> $$a²+a - b²-b = 0$$
> $$a²-b² = b-a$$
> - On as une identité remarquable :
> $$(a-b)(a+b) = -(a-b)$$
> - Si $a \neq b$  alors $a-b \neq 0$
> - Donc si ce n'est pas 0, on a le droit de diviser par $a-b$
> $$\frac{\cancel{(a-b)}(a+b)}{\cancel{(a-b)}} = -\cancel{\frac{(a-b)}{(a-b)}}$$
> $${a+b} = -1$$
> - On as trouvé notre contradiction, l'addition de deux entiers strictement positifs ne peut être un nombre négatif.

#### Conclusion
- Si $(P \Rightarrow nonQ)$ est ``Faux``, alors $(P \Rightarrow Q)$ est `Vrai`
- Par l'Absurde nous avons démontré que l'énoncé est `Vrai`