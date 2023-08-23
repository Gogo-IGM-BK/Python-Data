# 📝 Exercice 1 : Statistiques de base
## Scénario:

Vous travaillez comme analyste de données dans une entreprise. Votre manager vous a fourni les scores de satisfaction des clients pour le dernier trimestre et vous souhaite en extraire des informations statistiques.

Scores de satisfaction des clients :

90,85,88,78,92,84,81,79,95,8690,85,88,78,92,84,81,79,95,86

## Objectifs:

1. Créez un tableau Numpy pour ces scores.
2. Calculez la moyenne, la médiane et l'écart-type de ces scores.
3. Déterminez le score le plus élevé et le plus bas.

## Solution:
<details>
  <summary>Cliquez pour afficher le contenu caché</summary>

  ```python
    import numpy as np

    # 1. Créer un tableau Numpy
    scores = np.array([90, 85, 88, 78, 92, 84, 81, 79, 95, 86])
    
    # 2. Moyenne, médiane et écart-type
    moyenne = np.mean(scores)
    mediane = np.median(scores)
    ecart_type = np.std(scores)
    
    print(f"Moyenne : {moyenne}")
    print(f"Médiane : {mediane}")
    print(f"Ecart-type : {ecart_type:.2f}")
    
    # 3. Score le plus élevé et le plus bas
    print(f"Score le plus élevé : {np.max(scores)}")
    print(f"Score le plus bas : {np.min(scores)}")

  ```
</details>


