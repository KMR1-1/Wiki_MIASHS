## Définition

> [!note] Quand x peut avoir plusieurs valeurs et que le [[Raisonnement direct]] ne suffit pas à démontrer la propriété pour chacun des cas de x, on doit faire un raisonnement direct pour chaque cas de x.

## Exemple
- Pour tout réel x, la valeur absolue de $x-1$ est inferieur ou égale à $x²+x-1$
- $\forall x \in \mathbb{R}$, $|x-1|\leq x²+x-1$
- Ici les résultats sont différents selon si $x$ est positif ou négatif.
- On fait un raisonnement direct pour chaque cas.

>[!example] Cas 1 : Si $x \geq 1$ alors $|x-1| = (x-1)$
>- $(x-1)\leq x²+x-1$
>- $0 \leq x²+x-1 - (x-1)$
>- $0 \leq x² \Rightarrow Vrai$

> [!example] Cas 2 : Si $x < 0$ alors $|x-1| = -(x-1)$
>- $-(x-1)\leq x²+x-1$
>- $0 \leq x²+x-1 + (x-1)$
>- $0 \leq x² + 2x + 1 + 1$
>- $0 \leq (x-1)² +1 \Rightarrow Vrai$

- La propriété est Vrai pour ces deux cas de figure !