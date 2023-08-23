# 📝 Exercice 2 : Opérations Matricielles
## Scénario:

Vous êtes un ingénieur en robotique et travaillez sur la transformation de coordonnées. Vous avez deux matrices A et B et vous devez effectuer certaines opérations matricielles.

Matrices:

AA = [1,2],[3,4][1,2],[3,4]

BB = [2,2],[2,2][2,2],[2,2]

## Objectifs:

    Multipliez les deux matrices (multiplication matricielle).
    Calculez l'inverse de la matrice A.
    Calculez le déterminant de la matrice B.

Solution:
<details>
  <summary>Cliquez pour afficher le contenu caché</summary>

  ```python
    import numpy as np

    # 1. Créer les matrices A et B
    A = np.array([[1, 2], [3, 4]])
    B = np.array([[2, 2], [2, 2]])
    
    # 2. Multiplication matricielle
    resultat = np.dot(A, B)
    print(f"Multiplication de A et B:\n{resultat}")
    
    # 3. Inverse de la matrice A
    inverse_A = np.linalg.inv(A)
    print(f"Inverse de A:\n{inverse_A}")
    
    # 4. Déterminant de la matrice B
    determinant_B = np.linalg.det(B)
    print(f"Déterminant de B: {determinant_B:.2f}")

  ```
</details>
