##Exercice : 

Analyse des ventes d'une boutique en ligne

Vous travaillez pour une boutique en ligne et on vous fournit un ensemble de données contenant des informations sur les ventes de produits au cours du dernier mois. Votre tâche consiste à analyser ces données pour obtenir des informations utiles pour l'entreprise.

Données fournies :

` ventes.csv ` :

```
Date,Produit,Prix_unitaire,Quantité,Ville
01/08/2023,Ordinateur,800,5,Paris
01/08/2023,Chaise,50,10,Lyon
02/08/2023,Ordinateur,800,3,Marseille
02/08/2023,Table,200,7,Paris
03/08/2023,Chaise,50,5,Lyon
03/08/2023,Ordinateur,800,6,Marseille

```

Objectifs :

1. Lire le fichier CSV et le transformer en DataFrame.
2. Calculer le chiffre d'affaires total.
3. Trouver le produit le plus vendu.
4. Afficher le chiffre d'affaires par ville.

## Solution :
<details>
  <summary>Cliquez pour afficher le contenu caché</summary>
  
  ```python
    import pandas as pd

    # 1. Lire le fichier CSV et le transformer en DataFrame.
    df = pd.read_csv('ventes.csv')
    
    # 2. Calculer le chiffre d'affaires total.
    df['Chiffre_daffaires'] = df['Prix_unitaire'] * df['Quantité']
    chiffre_daffaires_total = df['Chiffre_daffaires'].sum()
    print(f"Chiffre d'affaires total : {chiffre_daffaires_total}€")
    
    # 3. Trouver le produit le plus vendu.
    produit_plus_vendu = df.groupby('Produit')['Quantité'].sum().idxmax()
    print(f"Produit le plus vendu : {produit_plus_vendu}")
    
    # 4. Afficher le chiffre d'affaires par ville.
    chiffre_daffaires_par_ville = df.groupby('Ville')['Chiffre_daffaires'].sum()
    print(chiffre_daffaires_par_ville)

  ```

</details>
