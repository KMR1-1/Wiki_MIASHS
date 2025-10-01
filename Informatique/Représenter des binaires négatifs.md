### Représenter un nombre négatif
- Au lieu d'aller de 0 à 255 en 8bit, on décale tout de la moitié
	- Ce qui permet de représenter des entiers de −128 à +127.
![[bit negatif]]
- Les nombres de ``0000 0000`` à ``0111 1111`` sont positifs, au delà de ça (de ``1000 0000`` à ``1111 1111``) ils sont négatifs.


> [!hint] Conversion Négative
> 1. **Convertir ``48`` en binaire** :
>     - 48 -> `00110000`
> 2. **Inverser les bits** :
> 	- 0->1 et 1->0
>     - `00110000` -> `11001111`
> 3. **Ajouter 1** :
>     - `11001111` + `1` = `11010000` 
>     - ``11010000`` représente -48 en binaire


- Si j'ai `11010000` mais que je ne sais pas ce qu'il représente en décimal : je fais la même opération.

> [!hint] Conversion Positive
> 1. **Inverser `11010000`** :
> 	- `11010000` -> `00101111` 
> 2. **Ajouter 1** :
> 	- ``0010111`` + ``1`` = ``00110000``
> 3. **Convertir en décimales**
> 	- `00110000` -> ``48``
> 	- Donc ``11010000`` -> `-48`
