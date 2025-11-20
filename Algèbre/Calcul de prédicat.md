# Règles de base

> [!hint] Distributivité logique
> 
>- $non (P \cap Q) \Leftrightarrow (non P) \cup (non Q)$
>- $non (P \cup Q) \Leftrightarrow (non P) \cap (non Q)$
> ---
>- $P \cap (Q \cup R) \Leftrightarrow (P \cap Q) \cup (P \cap R)$
>- $P \cup (Q \cap R) \Leftrightarrow (P \cup Q) \cap (P \cup R)$
>---
>- $(P \Rightarrow Q) \Leftrightarrow ( non P \Rightarrow non Q )$

# Raisonnements

Quand on veux chercher à démontrer un [[Quantificateurs#Enoncé|énoncé]], on procède par plusieurs types de raisonnements :

Types de Raisonnements
[[Raisonnement direct]]
	Prouve qu'une propriété est Vraie grâce à une égalité.
[[Raisonnement cas par cas]]
	Selon les cas de figure de la propriété, on prouve qu'elle est Vraie grâce à plusieurs égalités.
[[Raisonnement par Contraposée]]
	Prouver qu'une implication est Vraie ou Fausse grâce à sa contraposée.
[[Raisonnement par l'Absurde]]
	Si on nie une implication, trouver une contradiction au fait de la nier prouve que la propriété est Vraie.
[[Raisonnement par Contre Exemple]]
	Si on fait la négation d'une propriété
	Si cette négation est Vraie, c'est un contre exemple à la propriété.
	Si cette négation est Fausse, cela prouve la propriété.

---
# Logique de négation

> [!info] 
>- Quand on introduit une variable, l'égalité reste la ême
>- Pour les variables, les égalités s'inversent

| P                          | non P                      |
| -------------------------- | -------------------------- |
| $\exists x \in \mathbb{R}$ | $\forall x \in \mathbb{R}$ |
| $x = y$                    | $x \neq y$                 |
| $x \in \mathbb{R}$         | $x \notin \mathbb{R}$      |
| $<$                        | $\geq$                     |
| $>$                        | $\leq$                     |
| $\in$                      | $\notin$                   |
### Exemple de négation

> [!NOTE] Négation d'une équivalence
> - On va utiliser les règles établies au dessus pour trouver la négation d'une équivalence.
> - On sait que $(Q \Leftrightarrow P)$ est équivalent à ==$(Q \Rightarrow P) \cap (P \Rightarrow Q)$==
> - Donc $non[(Q \Rightarrow P) \cap (P \Rightarrow Q)]$ est équivalent à ==$non(Q \Rightarrow P) \cup non(P \Rightarrow Q)$==
> 	- On voit que $\cap$ est devenu $\cup$
> - On sais que $(P \Rightarrow Q)$ est équivalent à $(nonP \cup Q)$
> 	- On va donc remplacer les termes
> - Donc $non(Q \Rightarrow P) \cup non(P \Rightarrow Q)$ équivaux à $non(nonQ \cup P) \cup non(nonP \cup Q)$
> 	- $non(nonQ \cup P)$ nous donne $[non(nonQ) \cap (nonP)]$ soit $(Q \cap nonP)$
> 	- $non(nonP \cup Q)$ nous donne $[non(nonP) \cap (nonQ)]$ soit $(P \cap nonQ)$
>- On remet ça au propre : $(Q \cap nonP) \cup (P \cap nonQ)$
> - On sais maintenant que $non(Q \Leftrightarrow P) \Leftrightarrow (Q \cap nonP) \cup (P \cap nonQ)$

> [!question] Annulation Logique : Supposons $0 \leq x < 2$
> - non $(0 \leq x < 2)$
>- <=> non ( $(2 > x) \cap (x \geq 0)$ )
> - <=> (non $(2 > x)$) $\cup$ (non $(x \geq 0)$)
> - <=> ($x \geq 2) \cup (x < 0)$
	
> [!info] Annulation intuitive
> - Ici x est dans l'ensemble $[0;2[$
 >- La négation intuitive de cet intervalle, c'est tout ce qui n'est pas dans dedans, soit :
 >- $]-\infty \space; 0[ \space \cup \space ]2 \space;+\infty[$
 >- Mais on peut le trouver par les règles de logique
 
 
 