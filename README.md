
# 🐍 Introduction à Python

## 🏷️ Variables et types de données

En Python, une variable est un conteneur pour une valeur. Python supporte différents types de données, notamment :

- **Integers** : Ce sont des nombres entiers. Par exemple, `x = 10`. 🧮
- **Floats** : Ce sont des nombres à virgule flottante. Par exemple, `y = 20.5`. 🔢
- **Strings** : Ce sont des séquences de caractères. Par exemple, `z = "Bonjour"`. 📝
- **Booleans** : Ils représentent soit True (vrai), soit False (faux). Par exemple, `a = True`. ✅

## ➕➖✖️➗ Opérations de base

Python offre de nombreuses opérations de base, comme l'addition (`+`), la soustraction (`-`), la multiplication (`*`), et la division (`/`). Par exemple, si `x = 10` et `y = 20`, alors `x + y` donnerait `30`.

## 🔄 Structures de contrôle : boucles et instructions conditionnelles

Les structures de contrôle en Python comprennent les boucles `for` et `while`, ainsi que les instructions conditionnelles `if`, `elif`, et `else`.

- **Boucles** : Par exemple, `for i in range(5): print(i)` affichera les nombres de 0 à 4. 🔁
- **Instructions conditionnelles** : Par exemple, 
```python
x = 10
if x > 0:
    print("x est positif")
elif x < 0:
    print("x est négatif")
else:
    print("x est zéro")
🔀
```


## 🎁 Fonctions
En Python, une fonction est un bloc de code réutilisable qui effectue une action spécifique. Par exemple :
```python
def saluer(nom):
    print(f"Bonjour, {nom}!")

saluer("Alice")
👋
```
### Fonctions Lambda
Les fonctions lambda sont des petites fonctions anonymes. Elles peuvent prendre n'importe quel nombre d'arguments, mais peuvent seulement avoir une seule expression. Par exemple :
```python
x = lambda a : a + 10
print(x(5))  # affiche 15

```

Dans cet exemple, `x` est une fonction lambda qui prend un argument `a` et renvoie `a + 10`. Quand nous appelons `x(5)`, elle renvoie `15`.

## 📦 Modules et paquets

Un module en Python est un fichier contenant du code Python. Un paquet est une façon d'organiser les modules Python. Par exemple, vous pouvez importer le module math pour accéder à des fonctions mathématiques :

```python
import math
print(math.sqrt(16))  # affiche 4.0

➗
```








