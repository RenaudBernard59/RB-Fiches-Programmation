# Fiche programmation

## Algorithmique
### Introduction


### Hello World

### Commentaires
Généralement
// Une Seule Ligne
/* Sur
Plusieurs
lignes */

### Variables
#### Déclaration de variables
var TYPE maVariable := Valeur
var TYPE maVariable <- Valeur

#### Déclaration de constantes
const maCst = val TYPE
const pi = 3.14 REAL


#### Types de variables
##### Variables Numériques
* Entier | INT | 0, 4, 12, 1234, 9974116546
* Réel | REAL | 1.5, 3.1416 | 0.0000000000002 | 4589.166894109



##### Variables Textuelles
* Carctère | CAR | 'a', 't', 'm', 'G', '&', '?''
* Chaine de caractère | STR | 'Hello', 'World', 'Hello World!', 'Coucou \n Beuh!'


##### Variables Booléennes
* Vrais | TRUE
* Faux | FALSE

##### Variables Tableau
VAR identificateur :






### Expressions
* Opérateurs arithmétique + - * / %
* Opérateurs logiques NON ! OU || et &&
* Opérateurs relationnels = < > <= => 
* Opérateurs sur les chaines & © concaténation
Alt+0169

### Priorité des opérateurs
1. () Parenthèses
2. ^ élévation à la puissance
3. * / multiplications et divisions
4. + - additions et soustractions

Table de vérité

| A | B | A AND B | A OR B |
| T | T | T | T |
| T | F | F | T |
| F| T | F | T |
| F | F | F | F |

### Instructions conditionnelles

SI condition ALORS
    Suite d'instruction
SINON
    Suite d'instruction
FINI

SI condition ALORS
    Suite d'instruction
SINON SI condition ALORS
    Suite d'instruction
SINON SI condition ALORS
    Suite d'instruction
SINON
    Suite d'instruction
FINI

CAS OU ma Variable VAUT
    1 : faireCa
    2 : faireCa
    3 : faireCa
    4 : faireCa
    Autre : faireCa

var caractere
DEBUT
    SI caractere >= 'A' && caractere <='Z'
        CAS OU caractere vaut 'A', 'E', 'I', 'O', 'U', 'Y'
            ECRIRE("C'est une voyelle")
        FINCAS
    SINON
        ECRIRE("ce n'est pas une majusccule")
    FINSI
FIN

### Boucles

TANTQUE condition
    instruction
FIN TANTQUE

REPETER
    instruction
JUSQU'A condition

POUR compteur ALLANT DE début A fin FAIRE
    instruction
FIN POUR

### Fonctions
FONCTION maFonction(parametres)
DEBUT
    instructions
    Retourner(resultat)
FIN






===============================================================================
**Examples**

```JavaScript
Contenu
```

```Python
Contenu
```

```Ruby
Contenu
```

```PHP
Contenu
```

```C
Contenu
```

```C++
Contenu
```

```C#
Contenu
```

```Java
Contenu
```

```Cobol
Contenu
```

```Fortan
Contenu
```

```VBA
Contenu
```



