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
## Les 30 fonctions les plus utilisées dans Numpy 

| Fonction	     |Description	Exemple                                                     |                                      |
|----------------|------------------------------------------------------------------------|--------------------------------------|
|np.array()  	   |Crée un tableau numpy.                                                  |np.array([1, 2, 3])                   |
|np.zeros()	     |Renvoie un tableau rempli de zéros.	                                    |np.zeros((3,3))|
|np.ones()  	   |Renvoie un tableau rempli de uns.	                                      |np.ones((3,3))|
|np.full()  	   |Renvoie un tableau rempli de la valeur donnée.	                        |np.full((3,3), 7)|
|np.eye()	       |Renvoie une matrice identité de taille spécifiée.	                      |np.eye(3)|
|np.arange()	   |Renvoie des valeurs régulièrement espacées dans un intervalle donné.	  |np.arange(0, 10, 2)|
|np.linspace()   |Renvoie un nombre spécifié de valeurs régulièrement espacées entre deux valeurs données.	|np.linspace(0, 1, 5)|
|np.reshape()	   |Donne une nouvelle forme à un tableau sans changer ses données.	        |np.reshape(a, (2,3))|
|np.flatten()	   |Renvoie une copie aplatie d'un tableau donné.	                          |a.flatten()|
|np.append()	   |Ajoute des valeurs à la fin d'un tableau.	                              |np.append(a, [1,2])|
|np.delete()	   |Renvoie un nouveau tableau avec certains éléments supprimés.	          |np.delete(a, [1,2])|
|np.concatenate()|Joint une séquence de tableaux le long d'un axe existant.	              |np.concatenate((a, b), axis=0)|
|np.split()	     |Divise un tableau en plusieurs sous-tableaux.	                          |np.split(a, 3)|
|np.add()	       |Additionne les éléments de deux tableaux.	                              |np.add(a, b)|
|np.subtract()	 |Soustrait les éléments du deuxième tableau à partir du premier.	        |np.subtract(a, b)|
|np.multiply()	 |Multiplie les éléments de deux tableaux.	                              |np.multiply(a, b)|
|np.divide()	   |Divise les éléments du premier tableau par les éléments du second.	    |np.divide(a, b)|
|np.power()	     |Elève les éléments du premier tableau à des puissances du deuxième tableau.	|np.power(a, 2)|
|np.sqrt()	     |Renvoie la racine carrée des éléments du tableau.	                      |np.sqrt(a)|
|np.sin(), np.cos(), np.tan()	|Fonctions trigonométriques.	                              |np.sin(a)|
|np.log(), np.log10(), np.exp()	|Fonctions logarithmiques et exponentielles.	            |np.log(a)|
|np.sum()	      |Calcule la somme des éléments du tableau.	                              |np.sum(a)|
|np.mean()	    |Calcule la moyenne des éléments du tableau.	                            |np.mean(a)|
|np.median()	  |Calcule la médiane des éléments du tableau.	                            |np.median(a)|
|np.std()	      |Calcule l'écart-type des éléments du tableau.	                          |np.std(a)|
|np.sort()	    |Renvoie un tableau trié.	                                                |np.sort(a)|
|np.argmax(), np.argmin()	|Renvoient l'index de l'élément maximal/minimal d'un tableau.	  |np.argmax(a)|
|np.unique()	  |Trouve les éléments uniques d'un tableau.	                              |np.unique(a)|
|np.where()	    |Renvoie les indices où une condition donnée est vraie.	                  |np.where(a > 0)|
|np.random.rand(), np.random.randint()	| Génèrent des nombres aléatoires.	              |np.random.rand(5)|

Numpy est une bibliothèque très riche avec de nombreuses autres fonctionnalités. Assurez-vous de consulter la documentation officielle pour en savoir plus !


