# Règles de base

- Voici des exemples d'égalité d'[[Opérateurs Logiques]]

> [!hint] Exemples d'équivalence entre des Assertions
> 
>- $non (P \cap Q) \Leftrightarrow (non P) \cup (non Q)$
>- $non (P \cup Q) \Leftrightarrow (non P) \cap (non Q)$
> ---
>- $P \cap (Q \cup R) \Leftrightarrow (P \cap Q) \cup (P \cap R)$
>- $P \cup (Q \cap R) \Leftrightarrow (P \cup Q) \cap (P \cup R)$
>---
>- $(P \Rightarrow Q) \Leftrightarrow ( non P \Rightarrow non Q )$

# Raisonnements

- Quand on veux chercher à démontrer un énoncé, on procède par plusieurs types de raisonnements :

> [!NOTE] Types de Raisonnements
> - [[Raisonnement direct]]
> 	- Prouve qu'une propriété est Vraie grâce à une égalité.
> - [[Raisonnement cas par cas]]
> 	- Selon les cas de figure de la propriété, on prouve qu'elle est Vraie grâce à plusieurs égalités.
> - [[Raisonnement par Contraposée]]
> 	- Prouver qu'une implication est Vraie ou Fausse grâce à sa contraposée.
> - [[Raisonnement par l'Absurde]]
> 	- Si on nie une implication, trouver une contradiction au fait de la nier prouve que la propriété est Vraie.
> - [[Raisonnement par Contre Exemple]]
> 	- Si on fait la négation d'une propriété
> 		- Si cette négation est Vraie, c'est un contre exemple à la propriété.
> 		- Si cette négation est Fausse, cela prouve la propriété.

---
# Logique de négation

> [!info] 
>- Les [[Quantificateurs]] s'opposent, les ensembles restent les mêmes
>- Pour les variables, les égalités s'inversent

| P                          | non P                      |
| -------------------------- | -------------------------- |
| $\exists x \in \mathbb{R}$ | $\forall x \in \mathbb{R}$ |
| $x = y$                    | $x \neq y$                 |
| $x \in \mathbb{R}$         | $x \notin \mathbb{R}$      |
| $<$                        | $\geq$                     |
| $>$                        | $\leq$                     |
### Exemple de négation
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
 