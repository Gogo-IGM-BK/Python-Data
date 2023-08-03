# 🔢 Introduction à Numpy

[Numpy](https://numpy.org/) est une bibliothèque Python utilisée pour le calcul numérique. Elle permet de travailler avec des données sous forme de tableaux multidimensionnels (ndarrays) et fournit une grande variété de fonctions mathématiques performantes.

## 💾 Installation

Si vous n'avez pas encore installé Numpy, vous pouvez le faire en utilisant pip :

```bash
pip install numpy
```

## 🧮 Travailler avec des tableaux Numpy

Voici comment vous pouvez créer un tableau Numpy et effectuer des opérations de base :

```python
import numpy as np

# Créer un tableau Numpy
a = np.array([1, 2, 3, 4, 5])

# Afficher le tableau
print(a)  # Affiche : [1 2 3 4 5]

# Effectuer des opérations mathématiques sur le tableau
print(a + 2)  # Ajoute 2 à chaque élément : [3 4 5 6 7]

```

## 📊 Opérations de base avec Numpy

Numpy fournit une grande variété de fonctions pour effectuer des opérations sur des tableaux, comme des opérations arithmétiques, des opérations matricielles, des opérations logiques, etc.

Voici quelques exemples :

```python
import numpy as np

a = np.array([1, 2, 3, 4, 5])
b = np.array([6, 7, 8, 9, 10])

# Addition
print(a + b)  # Affiche : [ 7  9 11 13 15]

# Soustraction
print(a - b)  # Affiche : [-5 -5 -5 -5 -5]

# Multiplication
print(a * b)  # Affiche : [ 6 14 24 36 50]

# Division
print(a / b)  # Affiche : [0.16666667 0.28571429 0.375 0.44444444 0.5]

```
## 🔍 Indexation et slicing avec Numpy

Numpy offre des fonctionnalités puissantes pour indexer et slicer des tableaux :

```python
import numpy as np

a = np.array([1, 2, 3, 4, 5])

# Indexation
print(a[0])  # Affiche : 1

# Slicing
print(a[1:4])  # Affiche : [2 3 4]
```

Numpy est une bibliothèque très riche avec de nombreuses autres fonctionnalités. Assurez-vous de consulter la documentation officielle pour en savoir plus !


