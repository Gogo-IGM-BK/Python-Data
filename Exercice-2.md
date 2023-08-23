##Exercice : 

Analyse approfondie des ventes d'une chaîne de magasins

Vous êtes analyste de données pour une grande chaîne de magasins ayant plusieurs boutiques à travers le pays. On vous fournit un ensemble de données des ventes de ces boutiques pour l'année écoulée. Votre mission est de fournir des analyses approfondies pour aider la direction à prendre des décisions éclairées.

Données fournies :

ventes.csv :

```
Date,Produit,Catégorie,Prix_unitaire,Quantité,Boutique,Ville,Région
01/01/2023,Ordinateur,Électronique,800,5,Boutique1,Paris,Île-de-France
02/01/2023,Chaise,Mobilier,50,10,Boutique2,Lyon,Auvergne-Rhône-Alpes
02/01/2023,Table,Mobilier,200,7,Boutique3,Marseille,Provence-Alpes-Côte d'Azur

```
##Objectifs :

1. Lire le fichier CSV et le transformer en DataFrame.
2. Calculer le chiffre d'affaires mensuel pour toute l'année.
3. Trouver la catégorie de produits qui génère le plus de revenus.
4. Identifier la boutique avec le moins de ventes en termes de quantité et proposer des raisons possibles.
5. Afficher les 3 régions avec le plus grand chiffre d'affaires.
6. Pour la région ayant le plus grand chiffre d'affaires, afficher une répartition mensuelle des ventes.

##Solution :

<details>

  ```python
  import pandas as pd

  # 1. Lire le fichier CSV et le transformer en DataFrame.
  df = pd.read_csv('ventes.csv')
  df['Date'] = pd.to_datetime(df['Date'])
  
  # 2. Calculer le chiffre d'affaires mensuel pour toute l'année.
  df['Chiffre_daffaires'] = df['Prix_unitaire'] * df['Quantité']
  chiffre_daffaires_mensuel = df.groupby(df['Date'].dt.month)['Chiffre_daffaires'].sum()
  print(chiffre_daffaires_mensuel)
  
  # 3. Trouver la catégorie de produits qui génère le plus de revenus.
  categorie_top = df.groupby('Catégorie')['Chiffre_daffaires'].sum().idxmax()
  print(f"Catégorie la plus rentable : {categorie_top}")
  
  # 4. Identifier la boutique avec le moins de ventes en termes de quantité.
  boutique_moins_ventes = df.groupby('Boutique')['Quantité'].sum().idxmin()
  print(f"Boutique avec le moins de ventes : {boutique_moins_ventes}")
  # (Pour proposer des raisons possibles, une analyse plus approfondie des données et du contexte serait nécessaire)
  
  # 5. Afficher les 3 régions avec le plus grand chiffre d'affaires.
  top_regions = df.groupby('Région')['Chiffre_daffaires'].sum().nlargest(3)
  print(top_regions)
  
  # 6. Pour la région ayant le plus grand chiffre d'affaires, afficher une répartition mensuelle des ventes.
  region_max = top_regions.idxmax()
  ventes_region_max = df[df['Région'] == region_max].groupby(df['Date'].dt.month)['Chiffre_daffaires'].sum()
  print(f"Répartition mensuelle des ventes pour {region_max} :")
  print(ventes_region_max)

  ```
</details>
