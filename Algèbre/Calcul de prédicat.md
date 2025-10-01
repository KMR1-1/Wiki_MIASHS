# Règles de base 
- [[Opérateurs Logiques]]

> [!hint] Exemples d'équivalence entre des Assertions
> 
>- non (P et Q) <=> (non P) ou (non Q)
>- non (P ou Q) <=> (non P) et (non Q)
> ---
>- P et (Q ou R) <=> (P et Q) ou (P et R)
>- P ou (Q et R) <=> (P ou Q) et (P et R)
>---
>- (P => Q) <=> ( (non P) => (non Q) )

- Quand on veux chercher à démontrer un énoncé, on procède par plusieurs types de raisonnements :
	- [[Raisonnement direct]]
	- [[Raisonnement cas par cas]]
	- [[Raisonnement par Contraposée]]
	

---
# Logique d'annulation des prédicats

> [!info] 
>- Pour les [[Quantificateurs]], les égalités restent les mêmes
>	- Seul les quantificateurs s'opposent
>- Pour les variables, les égalités s'inversent

| P                          | non P                      |
| -------------------------- | -------------------------- |
| $\exists x \in \mathbb{R}$ | $\forall x \in \mathbb{R}$ |
| $x = y$                    | $x \neq y$                 |
| $x \in \mathbb{R}$         | $x \notin \mathbb{R}$      |
| $<$                        | $\geq$                     |
| $>$                        | $\leq$                     |
### Exemple d'annulation de logique
- Supposons $0 \leq x < 2$

> [!question] Annulation Logique
> - non $(0 \leq x < 2)$
>- <=> non ( $(2 > x) \cap (x \geq 0)$ )
> - <=> (non $(2 > x)$) $\cup$ (non $(x \geq 0)$)
> - <=> ($x \geq 2) \cup (x < 0)$
	
> [!info] Annulation intuitive
> - Ici x est dans l'ensemble $[0;2[$
 >- La négation intuitive de cet intervalle, c'est tout ce qui n'est pas dans dedans, soit :
 >- $]-\infty \space; 0[ \space \cup \space ]2 \space;+\infty[$
 >- Mais on peut le trouver grâce a la logique
 