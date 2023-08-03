# 📚 Structures de données Python

## 📝 Listes

En Python, une liste est une collection ordonnée et modifiable d'éléments. Par exemple :

```python
ma_liste = [1, 2, 3, "Python", "Data"]
```
Chaque élément dans une liste a un index, qui commence à 0.

## 🧩 Tuples
Un tuple est une collection ordonnée et non modifiable d'éléments. Par exemple :

```python
mon_tuple = (1, 2, 3, "Python", "Data")
```
Comme les listes, chaque élément dans un tuple a un index, qui commence à 0.


## 📖 Dictionnaires
Un dictionnaire est une collection non ordonnée, modifiable et indexée d'éléments. Il est écrit avec des accolades, et ils ont des clés et des valeurs. Par exemple :

```python
mon_dictionnaire = {"langage": "Python", "sujet": "Data"}

```

## 🎁 Ensembles
Un ensemble est une collection non ordonnée et non indexée d'éléments. En Python, les ensembles sont écrits avec des accolades. Par exemple :

```python
mon_ensemble = {1, 2, 3, "Python", "Data"}

```
Notez que les ensembles ne peuvent pas avoir de doublons - chaque élément doit être unique.

## Brève comparaison entre les différentes structures :

### Listes :

- Collections ordonnées et modifiables.
- Peuvent contenir différents types de données (int, float, string, etc.) et d'autres listes.
- Les éléments peuvent être dupliqués.
- Sont définies par des crochets [ ].

### Tuples :

- Collections ordonnées et non modifiables.
- Peuvent contenir différents types de données.
- Les éléments peuvent être dupliqués.
- Sont définies par des parenthèses ( ).

### Dictionnaires :

- Collections non ordonnées, modifiables et indexées.
- Les dictionnaires sont composés de paires clé-valeur.
- Les clés sont uniques tandis que les valeurs peuvent être dupliquées.
- Sont définies par des accolades { } avec les éléments séparés par des virgules et les paires clé-valeur sont séparées par des deux-points :. Par exemple, {'clé1' : 'valeur1', 'clé2' : 'valeur2'}.

### Ensembles :

- Collections non ordonnées et non indexées.
- Ne contiennent pas de doublons.
- Sont également définis par des accolades { }, mais sans les deux-points pour séparer les clés et les valeurs comme dans les dictionnaires.
- Les ensembles sont utiles pour vérifier l'appartenance d'un élément et pour éliminer les éléments en double.

## Cas d'utilisation

### Listes :

- Utilisées lorsque l'ordre des éléments est important et que ces éléments sont modifiables.
- Utiles pour stocker une collection d'items similaires, ou si vous avez besoin de dupliquer des éléments.
- Les listes sont très utilisées dans les boucles pour parcourir une séquence d'éléments.

### Tuples :

- Utilisés lorsque l'ordre des éléments est important mais que ces éléments ne sont pas modifiables.
- Utilisés lorsque vous voulez rendre certains éléments immuables, par exemple, les coordonnées d'un point dans un espace 2D ou 3D.

### Dictionnaires :

- Utilisés pour stocker des données sous forme de paires clé-valeur, ce qui est pratique lorsque vous avez besoin d'une association logique entre une clé et une valeur.
- Par exemple, pour stocker les informations d'un annuaire téléphonique où chaque nom (clé) est associé à un numéro de téléphone (valeur).

### Ensembles :

- Utilisés lorsque vous voulez stocker plusieurs éléments dans une seule variable, mais que vous ne voulez pas de doublons et que l'ordre des éléments n'est pas important.
- Utiles pour tester si un élément est présent dans le set ou non, car cette opération est plus rapide avec un ensemble qu'avec une liste.
- Par exemple, pour garder une liste unique de tags ou de catégories.
