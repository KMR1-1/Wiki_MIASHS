## Introduction à Java et Eclipse

### Eclipse

Eclipse est un **environnement de développement** :  
c’est l’endroit où l’on **écrit**, **exécute** et **teste** ses programmes Java.
### Programme, Classe et Java

- Un **programme** est un **fichier** sur ton ordinateur, par exemple : `MonProgramme.java`
    
- Ce fichier contient une **classe** qui porte **le même nom** :
    
    ```java
    public class MonProgramme {
        // le code ici
    }
    ```
    
- **Java** est le **langage** utilisé : il a ses propres règles et une syntaxe précise.  
    Chaque ligne que tu écris est une **instruction** que l’ordinateur exécutera.
    
### La méthode `main`

C’est le **point de départ** du programme :  
quand tu exécutes ton code, **tout ce qu’il y a entre les `{ }` de `main`** sera lu et exécuté.  
## Les instructions

Une **instruction**, c’est comme un ordre donné à un chien :

> “assis”, “couché”, “donne la patte”  
> Le programme suit **exactement** les ordres, **dans l’ordre écrit**.  
> Mais attention : Java **ne devine rien**, il faut **tout lui préciser**, ce n'est pas ChatGPT, java ne parle pas français !

- Un exemple d'instruction c'est `System.out.println("Bonjour !")`
	- Ca veut juste dire "affiche 'Bonjour !' dans le terminal"

```java
public static void main(String[] args) {
    System.out.println("Bonjour !");
}
```
### Le terminal

Le **terminal** affiche le **résultat** du programme, comme ici :

```
Bonjour !
```

---
## Résumé

| Élément        | Rôle                          |
| -------------- | ----------------------------- |
| Programme      | Le fichier `.java`            |
| Classe         | Contient le code du programme |
| Méthode `main` | Point d’entrée du programme   |
| Java           | Le langage utilisé            |
| Instruction    | Un ordre                      |
| Terminal       | Affiche les résultats         |

---
