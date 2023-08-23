# 🥧 Diagramme à secteurs (Pie chart):

```python
  import matplotlib.pyplot as plt

  labels = ['A', 'B', 'C', 'D']
  sizes = [15, 30, 45, 10]
  colors = ['gold', 'yellowgreen', 'lightcoral', 'lightskyblue']
  explode = (0.1, 0, 0, 0)  # Explose le 1er segment
  
  plt.pie(sizes, explode=explode, labels=labels, colors=colors,
  autopct='%1.1f%%', shadow=True, startangle=140)
  
  plt.axis('equal')  # Pour avoir un diagramme circulaire
  plt.title("Diagramme à secteurs")
  plt.show()
```
# 📊 Barres empilées (Stacked bar chart):

```python
  import numpy as np
  import matplotlib.pyplot as plt
  
  N = 5
  menMeans = (20, 35, 30, 35, 27)
  womenMeans = (25, 32, 34, 20, 25)
  
  ind = np.arange(N)    # Les emplacements des groupes
  width = 0.35       # Largeur des barres
  
  fig, ax = plt.subplots()
  
  p1 = ax.bar(ind, menMeans, width, color='r')
  p2 = ax.bar(ind, womenMeans, width, bottom=menMeans, color='b')
  
  ax.axhline(0, color='grey', linewidth=0.8)
  ax.set_ylabel('Scores')
  ax.set_title('Scores par groupe et par genre')
  ax.set_xticks(ind)
  ax.set_xticklabels(('G1', 'G2', 'G3', 'G4', 'G5'))
  ax.legend((p1[0], p2[0]), ('Hommes', 'Femmes'))
  
  plt.show()

```
