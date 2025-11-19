# Définition
- Les Quantificateurs permettent d'introduire une variable dans un énoncé

___
# Quantificateur $\forall$ "pour tout"
- "Pour chaque", "pour n'importe quel" ![[quantifForAll]]
> [!NOTE] Pour tout :
> - On introduit la variable, et on définis dans quel ensemble elle se trouve.
> - On peut ensuite déclarer une propriété
> - Si on trouve une seule exception, cela invalide le prédicat :
> 	- voir : [[Raisonnement par Contre Exemple]]

# Quantificateur $\exists$ "il existe"
![[exists]]

> [!NOTE] Il existe :
> - Ici il peut y avoir plusieurs solution de n répondant au prédicat.
> 	- Mais une seule réponse suffit à Valider l'énoncé
> 	- On cherche donc 1 cas ou c'est vrai !
> - "$\exists !n$" ici on dit qu'il existe un unique n solution de la propriété

___
# Exemple
- On peut traduire tout nos énoncés grâce à cette écriture algébrique, ex :
- Pour tout entier n, si n est pair, alors n² est pair :
-  $\forall n \in \mathbb{N}, (\exists k \in \mathbb{N}, n = 2k) \implies (\exists l \in \mathbb{N}, n² = 2l)$
- C'est sous la forme $P \Rightarrow Q$
> [!hint] On pourrais aussi écrire $(\forall n \in \mathbb{N}, \exists k \in \mathbb{N},\exists l \in \mathbb{N}), (n = 2k \implies n² = 2l)$
>- La chose à savoir est que l'ordre est important
>	- Avant d'écrire une implication, il faut définir la variable et ses contraintes.
>	- De plus l'ordre à une importance : Si on fait $n=2k$
>		- $n$ dépends de $k$, donc $\forall n$ vient avant $\exists k$

| Francais                                                                   | Algèbre                                                                                      | Type                                            |
| -------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------- | ----------------------------------------------- |
| - pour tout entier n<br>- il existe un entier k<br>- il existe un entier l | - $\forall n \in \mathbb{N}$<br>- $\exists k \in \mathbb{N}$<br>- $\exists l \in \mathbb{N}$ | Quantificateurs :<br>Introduisent les variables |
| n est pair*                                                                | $n = 2k$                                                                                     | Hypothèse (si)                                  |
| n² est pair                                                                | $n² = 2l$                                                                                    | Conclusion (alors)                              |
- Cet énoncé est vérifié grâce au [[Raisonnement direct]] et [[Raisonnement par Contraposée]]