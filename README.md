## 🐼 b. Pandas

Pandas est l'une des bibliothèques les plus populaires pour l'analyse de données en Python. Elle offre une variété de structures de données et de fonctions pour manipuler rapidement et efficacement des séries de données et des dataframes.

### 📘 Résumé :

- 📋 **DataFrame**: Une structure de données bidimensionnelle, semblable à une table de base de données, une feuille de calcul Excel, ou une table de données en R.
- 🔢 **Série**: Une structure de données unidimensionnelle, similaire à une colonne dans une feuille de calcul.
- 🔧 **Opérations de base**: La lecture de fichiers (comme CSV, Excel), la manipulation d'index, le tri des données, la sélection/modification/ajout/suppression des données.
- 📊 **Fonctions de groupage**: Pandas est très utile pour regrouper des données et appliquer des fonctions d'agrégation comme la somme, la moyenne, le maximum, etc.
- 🔗 **Jointures et fusions**: Avec Pandas, vous pouvez facilement combiner des dataframes, comme vous le feriez avec des bases de données SQL.
- 🕰 **Manipulation de séries temporelles**: Pandas offre des outils pour traiter des données qui sont indexées par le temps.
- 🧹 **Nettoyage de données**: Pandas offre de nombreuses fonctions pour nettoyer et prétraiter vos données, y compris la gestion des valeurs manquantes.

### 🚀 Exemples d'utilisation :

1. **Création d'un DataFrame**:
```python
import pandas as pd

data = {
    'prénoms': ['Sophie', 'Lucas', 'Emma', 'Gabriel'],
    'âges': [23, 34, 45, 56]
}

df = pd.DataFrame(data)
print(df)
```
2.📄 **Lecture d'un fichier CSV**:
```python
data = pd.read_csv('mon_fichier.csv')
```

3.🔍 **Sélection de données**:
```python
# Sélectionner une colonne par son nom
ages = df['âges']

# Sélectionner des lignes par leurs indices
sous_ensemble = df.iloc[1:3]
```

4.📈 **Grouper et agréger des données**:
```python
df.groupby('âges').count()
```

