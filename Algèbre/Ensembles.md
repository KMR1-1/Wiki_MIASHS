## Définitions
Ensemble Vide : $\emptyset$
$E = \{1,4,7\}$ 
 - $x \in \{1,4,7\}$
 - $P(E) = \{\{\emptyset\}, \{1\}, \{4\}, \{7\}, \{1,4\}, \{1,7\}, \{4,7\}, \{1,4,7\}\}$
 - $card(P(E)) = 2^n$ avec $n$ le nombre d'élément de $E$
	
$E = \{n \in \mathbb{N} \space | \space \exists k \in \mathbb{N}, n = 2k\}$
- $E = \{2, 4, 6, ... 2k\}$
___
## Propriétés
Si $x \in E$ et $E \subset F$
- $\forall x \in E \Rightarrow x \in F$

Si $E \subset F$ et $F \subset E$ alors $E = F$

$A \subset B$ alors $A \land B = A$

$A \lor B = B$ alors $A \subset B$

$A \subset B \Rightarrow \complement B \subset \complement A$

$E \setminus A = \{x \in E \mid x \notin A\}$
___
#### Produit cartésien
$\mathbb{R}² = \mathbb{R} \times \mathbb{R} = \{(x,y) \mid x,y \in \mathbb{R} \}$
- $[0,1] \times \mathbb{R} = \{(x,y) \mid 0 \leq x \leq 1\}$
- $[0,1] \times [0,1] \times [0,1] \times = \{(x,y,z) \mid 0 \leq x,y,z \leq 1\}$
___
## Applications
$f : E \rightarrow F$
- $x \in E$ et $f(x) \in F$
- $x \rightarrow f(x)$
___
#### Graphe : 
$\Gamma_f = \{(x,f(x)) \in E \times F \mid x \in E\}$
- l'ensemble des points dans un espace 2D, c'est le graph.
- $\Gamma_f = \{(x,f(x)) \in \mathbb{R} \times \mathbb{R} \mid f(x) = x²\}$
___
#### Restriction :
$A \subset E$ et $f : E \rightarrow F$
- $f_{\mid A} : A \rightarrow F$
___
#### Image directe :
$A \subset E$ et $f : E \rightarrow F$
- $f(A) = \{f(x) \in F \mid x \in A\}$
___
#### Image réciproque 
 $B \subset F$ et $f:E \rightarrow F$
	 - $f^{-1}(B) = \{x \in E \mid f(x) \in B\}$
	 - $f^{-1}(f(x)) = x$
	
- **Antécédent** :
	- $f(x) = x²$ avec $x \in \mathbb{N}$
	- Si $f(x) \in [0,100]$
	- $f^{-1}(\{y\}) = [0,10]$ 
	- $f^{-1}(y) = \{x_i\}$
		- C'est les antécédents de $y$ où $x² = y$ donc $\sqrt{y} = x$
#Corriger
___
#### Composition :
$f : E \rightarrow F$ et  $g : F \rightarrow G$
- $g \circ f : E \rightarrow G$
- $g \circ f(x) = g(f(x))$
___
#### Identité :
$id_E : E \rightarrow E$ soit $x \rightarrow x$ 
$id_E(x) = x$ 

$f:E \rightarrow F$ et $g:F \rightarrow E$ 
- $f \circ g = id_F$ 
- $g \circ f = id_E$ 
- $(g\circ f)^{-1}=f^{-1}\circ g^{-1}$
___
## Surjectif, Injectif, Bijectifs

#### Injectif
$\forall x, x' \in E, \space (f(x) = f(x') \implies x = x')$
___
#### Surjectif
$\forall y \in F, \space \exists x \in E, \space (y = f(x))$
___

### Bijection
Injectif et surjectif
$\forall y \in F, \space \exists !x \in E, \space (y = f(x))$
___

**Bijection réciproque :**
L'application $f$ est bijective s'il existe une application $g$ où $g \circ f = Id_E$ et $f \circ g = Id_F$
$g$ s'appelle la bijection réciproque de $f$ et est unique