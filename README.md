## 📊 Matplotlib

Matplotlib est une bibliothèque de visualisation de données en Python qui offre des outils pour créer une grande variété de graphiques statiques, animés et interactifs.

### 📘 Résumé :

- 📈 **Graphiques Basiques**: Vous pouvez créer des diagrammes à barres, des histogrammes, des diagrammes à secteurs, des nuages de points, et bien plus encore.
- 🖌 **Personnalisation**: Chaque aspect du graphique est personnalisable : couleurs, légendes, titres, axes, etc.
- 📏 **Contrôle des Axes**: Définissez les limites, les étiquettes, et le style de vos axes pour mieux mettre en valeur vos données.
- 🌐 **Intégration**: Intégration facile avec d'autres bibliothèques comme Pandas pour visualiser directement les dataframes.
- 📄 **Export**: Exportez vos graphiques sous différents formats (PNG, PDF, SVG, etc.) pour les utiliser dans des présentations, des articles ou des sites web.

### 🚀 Exemples d'utilisation :

1. **Création d'un simple graphique**:
```python
import matplotlib.pyplot as plt

x = [1, 2, 3, 4, 5]
y = [1, 4, 9, 16, 25]

plt.plot(x, y)
plt.title("Graphique simple")
plt.xlabel("Axe des x")
plt.ylabel("Axe des y")
plt.show()
```
2. 📊 **Histogramme**:
```python
import numpy as np

data = np.random.randn(1000)
plt.hist(data, bins=30, color="skyblue", edgecolor="black")
plt.title("Histogramme")
plt.xlabel("Valeur")
plt.ylabel("Fréquence")
plt.show()
```
2. 🔍  **Nuage de points (scatter plot)**:
```python
x = np.random.randn(100)
y = x + np.random.randn(100)

plt.scatter(x, y, color="red")
plt.title("Nuage de points")
plt.xlabel("Axe des x")
plt.ylabel("Axe des y")
plt.show()

```





