
**Caractère** : Prix, couleur...
**Individu** : Arbre, Français... 
**Population** : Foret, population française... ($N$)
**Effectif** : $n$ 
**Fréquence** : $f_i =\frac{n_i}{N}$ 

### Discret : $X = \{3, 7, ..., 4\}$
- Diagramme en baton :
- ![[Diagramme baton.png]]
- Fonction de répartition fréquence :
	- Fréquence cumulée ($f.c.$)
	- Effectifs cumulés ($eff.c.$)
- ![[FRepartitionDiscret.png]]

---
### Continu : $X = [0 ;100]$
- intervalles équiprobables
- Histogramme : 
- ![[Histgramme.png]]
- [[Tracer un histogramme]]
- Fonction de répartition :
- ![[FRepartitionContinu.png]]

---
## Mots-clés

**Quantitatif** : nombres
**Qualitatif** : attributs

**Mode** : ensemble des valeur avec le plus effectif
**Classe** : intervalle de la barre la plus haute d'un histogramme.

**Moyenne** : $m(x) = \frac{x_i \times n_i}{N}$
	Distributivité : $m(ax+ay+c) = a*m(x+y)$
	$m(ax+by) = a*m(x) + b*m(y)$
	Utiliser $c_i$ pour continu : moyenne entre bornes intervalles.
	Centre de gravité des représentations graphiques (bâtons, histo)

**Quantiles** : Coupe les valeurs par une proportion (q0.x)
**Médiane** (q0.5) : coupe en 2 valeurs.
	Si $n$ impair, médiane = $n/2 + 0.5$
	Si n pair, médiane = $\frac{(n/2) + (n/2 \space +1)}{2}$
	Fonction de répartition : médiane à $\leq$ 0.5
	[[Trouver Médiane continue]]
**Quartile** : 1 et 2 (q0.25 et q0.75)
**Décile** : (q0.1, q0.2, ... , q0.9)


**Variance**: 
	$\sigma² = Var(x)=m(x²) - m(x)²$
	$m(x²) = \frac{1}{N} \sum(x_i²\times n_i)$ 

**Ecart-type (standard-deviation)** :
	$\sigma = \sqrt{Var(x)}$
	$\sigma_{ax+b} = |a|\sigma_x$
		Augmenter toutes les valeurs de b ne fait rien
		Augmenter toutes les valeurs d'un facteur augmente $\sigma$ du facteur
	Si $\sigma = 1.98$ et je veux qu'il soit égal à $2$ alors
		$2/1.98 = 1.0101$
		Donc je dois multiplier tout les $x_i$ par $1.0101$

---

## Boites de Distributions

$IQ = q_{0.75} - q_{0.25}$
$a = q_{0.25} - 1.5IQ$
$b = q_{0.75} + 1.5IQ$
$x_a = min(x_i : x_i \geq a)$
	Valeur la plus petite au-dessus de $a$ 
$x_b = max(x_i : x_i \leq b)$
	Valeur la plus grande en dessous de $b$

**Valeurs extrêmes**: Valeurs en dehors de $[a,b]$

![[boxplot.png]]
