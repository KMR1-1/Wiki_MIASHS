# Liste des principales instructions java

Toutes les **instructions** se terminent par un **`;`**  
Java lit ton programme **ligne par ligne** et exécute chaque instruction **dans l’ordre**.
Si je met `//` au début d'une ligne, c'est un commentaire, le programme ignore cette ligne

---

##  Afficher du texte dans le terminal

```java
System.out.print("Bonjour !");
System.out.println("Bonjour avec retour à la ligne !");
```

Tout ce qui est entre les guillemets `" "` sera affiché.  
Pour **afficher une variable**, on utilise le `+` :

```java
System.out.println("Le résultat est " + nb);
```

---

## Déclarer une variable

```java
int nb = 5;
```

|Élément|Signification|
|---|---|
|`int`|type de la variable (entier)|
|`nb`|nom de la variable|
|`= 5`|valeur donnée à la variable|

Modifier la variable :

```java
nb = nb + 3; // nb vaut maintenant 8
```

### Entrer une variable dans le terminal
On utilise la classe du Scanner
```java
Scanner s = new Scanner(System.in)

int nb = s.nextInt() 
```
Quand il y as la fonction "s.nextInt()" le programme s'arrête, et le terminal attends que l'on rentre un entier.
nb va prendre la valeur de cet entier

---

## Types de variables

| Type      | Sert à stocker...                 | Exemple          | Scanner      |
| --------- | --------------------------------- | ---------------- | ------------ |
| `int`     | un entier                         | `5`              | nextInt()    |
| `double`  | un nombre à virgule               | `6.8`            | nextDouble() |
| `float`   | un autre type de nombre à virgule | `6.8f`           | nextFloat()  |
| `String`  | du texte                          | `"Bonjour"`      | nextLine()   |
| `char`    | une seule lettre                  | `'e'`            | nextLine()   |
| `boolean` | vrai ou faux                      | `true` / `false` | nextBoolean  |

---

## Tableau (liste de valeurs)

Je commence avec un tableau de string :
```java
String[] chiens = {"Rex", "Médor", "Truffe"};
```

Attention, l'index commence à 0

```java
System.out.println("Mon deuxième chien s'appelle " + chiens[1]);
```

Affichera : `Mon chien s'appelle Médor`

Si on ne définis pas ce qu'il y as dans le tableau on va par exemple :
Créer un tableau vide de 5 entiers :

```java
int[] tab = new int[5]; //"tab" est un nouveau tableau d'entier avec 5 cases
tab[2] = 27; // je mets 27 dans la 3ème case de "tab"
```

---

## Condition `if`

```java
int age = 18;

if (age >= 18) {
    System.out.println("Tu es majeur");
} else {
    System.out.println("Tu es mineur");
}
```

Le code entre `{ }` est exécuté **seulement si** la condition est vraie.
`Else` est la négation de ce qui est dans `if`.
On utilise `&&` pour la logique "ET"
On utilise `||` (Les touches``alt gr`` +`` 6``), pour la logique "OU"
On utilise `==` pour la logique "="
- Attention un seul `=` veut dire qu'on rentre la valeur dans une valable comme `x = 3`
Attention, il faut éviter de déclarer une variable à l'intérieur des `{ }` de if.
- Car le code se trouvant dans le `if` ne s'exécute pas tout le temps, donc la variable peut ne jamais être déclarée.

---

## Boucle `while`

Répète tout ce qui est entre `{ }` tant qu’une condition est vraie :
```java
while(condition){
	//instructions
}
```

Voici un exemple où une boucle while nous demande le jour du mois en boucle si Le jour n'est pas valide :
```java
Scanner s = new Scanner(System.in); //cré un Scanner
System.out.println("entre un jour du mois entre 1 et 31"); //Affiche du texte
jourDuMois = s.nextInt(); //Demande un nombre

while (jourDuMois < 1 || jourDuMois > 31) { 
	//si jourDuMois inferieur à 1 OU jourDuMois supérieur à 31
    System.out.println("Le nombre dois etre entre 1 et 31, réécris un nombre");
    jourDuMois = s.nextInt()
}
```
Si le "jourDuMois" est en dessous de 1 ou au dessus de 31
- La condition `(jourDuMois < 1 || jourDuMois > 31)`
Alors le programme demande de redéfinir `jourDuMois`
Si le nombre n'est pas entre 1 et 31 alors la boucle recommence du début, et donc redemande de définir `jourDuMois` !
Sinon on sors de la boucle si le `jourDuMois` est entre 1 et 31.

Dans cet exemple la boucle est une sécurité pour éviter de rentrer des valeurs interdites.

---
## Boucle `for`

C'est comme la boucle while mais plus compacte
Répète un nombre précis de fois ce qui est entre `{ }` :

```java
for (int i = 0; i < 5; i++) {
    System.out.println("i vaut " + i);
}
```

Sortie :
```
i vaut 0
i vaut 1
i vaut 2
i vaut 3
i vaut 4
```

| int i = 0 | i commence à 0                               |
| --------- | -------------------------------------------- |
| i++       | i augmente de 1 a chaque boucle              |
| i > 5     | la boucle s'arrête quand i est supérieur à 5 |
### Parcourir un tableau

Si je veux parcourir un tableau je peux utiliser `tab.length()`
- Ca représente le nombre de cases du tableau.
```java
int[] tab = new int[10]
for (int i = 5; i < tab.length(); i++) {
    tab[i] = i
}
```

Attention ici i est inferieur au nombre de cases
- Car si il y a 10 cases, les index du tableau vont de 0 à 9.
Dans l'exemple au dessus, on commence à l'index 5 du tableau.
- Si `i = 5`, alors `tab[i] équivaut tab[5]`.
- Si `tab.length() équivaut 10` alors `i < 10`.
- Le tableau se remplis jusqu'à l'index 9.

---

## Exemple complet de programme

```java
public class BonjourJava {
    public static void main(String[] args) {
        // Déclaration d'une variable
        int age = 20;

        // Condition
        if (age >= 18) {
            System.out.println("Tu es majeur !");
        } else {
            System.out.println("Tu es mineur !");
        }

        // Boucle
        for (int i = 1; i <= 3; i++) {
            System.out.println("Essai numéro " + i);
        }

        // Tableau
        String[] animaux = {"Chat", "Chien", "Lapin"};
        System.out.println("Mon animal préféré est le " + animaux[1]);
    }
}
```

Sortie :

```
Tu es majeur !
Essai numéro 1
Essai numéro 2
Essai numéro 3
Mon animal préféré est le Chien
```