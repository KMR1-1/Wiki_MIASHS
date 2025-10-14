## Définition

> [!NOTE] Déf
> - Permet d'associer des [[Logique Mathématique#Assertion / Proposition|propositions]] pour en former de nouvelles.
> - L'association de deux propositions avec un opérateur logique va créer une table de vérité,
> 	- On y voit tout les cas de figure des propositions.
> - S'entrainer à faire des tables de vérité en jouant avec les opérateurs logiques, permet d'intégrer intuitivement les [[Calcul de prédicat]]
> - On note P et Q des propositions Vraies ou Fausses.

#### Opérateur "ou"
- Peut se noter : "or", "⋃"

| P $\cup$ Q | V   | F   |
| ---------- | --- | --- |
| V          | V   | V   |
| F          | V   | F   |
- le OU exclusif noté XOR, $\oplus$, 
#### Opérateur "et"
- peut se noter : "and", "⋂", "&"

| P $\cap$ Q | V   | F   |
| ---------- | --- | --- |
| V          | V   | F   |
| F          | F   | F   |
#### Opérateur "non"
- peut se noter "not", "¬"
- $non P$ est Vrai si $P$ est ``Fausse``

| P         | V   | F   |
| --------- | --- | --- |
| $\lnot$ P | F   | V   |
#### Implication
- $P \Rightarrow Q$ 
- similaire à : non($P$) $\cup$ $Q$
- "Il faut que" : =>
- "il suffit que" : <=

| P => Q | V   | F   |
| ------ | --- | --- |
| V      | V   | F   |
| F      | V   | V   |
- Se base sur le concept de ``promesse`` (Si, Alors).

> [!question] Les cas de L'implication ex : "Si tu range ta Chambre => Je te donne du Gâteau" est une implication logique
> 1. Tu as rangé ta chambre => Tu as du gâteau.
> 	- (Vrai => Vrai) est  Vrai
> 2. Tu n'as pas rangé ta chambre => Tu n'as pas de gâteau.
> 	- Ma promesse n'est pas brisée l'implication est donc Vrai !
> 	- ( Faux => Faux ) est Vrai 
> 3. Tu n'as pas rangé ta chambre => Tu as du gâteau.
> 	- C'est le cas de figure de l'implication le plus contre-intuitif.
> 	- Mais il n'a jamais été dit que "si tu ne ranges pas ta chambre => tu n'aura pas de gâteau".
> 	- Alors dans ce cas de figure, aucune promesse n'a été rompue, l'implication est donc Vrai !
> 	- ( Faux => Vrai ) = Vrai 
> 
> 4. Si tu range ta chambre, et que tu n'a pas de Gâteau.
> C'est le seul cas de figure ou la promesse est rompue, l'assertion est donc Fausse.
> ( V => F = F )

- La [[Raisonnement par Contraposée|contraposée]] d'une implication : c'est $(P \Rightarrow Q) \Leftrightarrow (nonP \Rightarrow non Q)$
- Le [[Raisonnement par l'Absurde]] d'une implication c'est :
	- "$(P \Rightarrow Q)$ est Vrai" si "$(P \Rightarrow nonQ)$ est Faux".

#### Équivalence 
 - $P \Rightarrow Q$
 - similaire à : $(P \Rightarrow Q) \cap (Q \Rightarrow P)$
- "Si Q est faux alors P est faux" est une assertion ``Vraie``.

| P <=> Q | V   | F   |
| ------- | --- | --- |
| V       | V   | F   |
| F       | F   | V   |

