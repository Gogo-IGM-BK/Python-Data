# 1. Afficher une carte de base simple:

Un exemple simple pour débuter avec GeoViews est d'afficher une carte de base.
```python
import geoviews as gv
import geoviews.feature as gf
from bokeh.io import show, output_file

output_file("map.html")
tile = gv.tile_sources.Wikipedia
plot = gv.render(tile)
show(plot)

```
Cet exemple montre simplement les côtes du monde entier.

# 2. Points sur une carte:

Afficher des points de données sur une carte est une opération courante avec les données géospatiales.

```python
import geoviews as gv
import pandas as pd
import geoviews.feature as gf
from bokeh.io import show, output_file

# Créer un DataFrame simple avec des coordonnées
data = pd.DataFrame({
    'Longitude': [-0.1276, 2.3522, 12.4924],
    'Latitude': [51.5074, 48.8566, 41.9028],
    'City': ['London', 'Paris', 'Rome']
})

points = gv.Points(data, ['Longitude', 'Latitude'], ['City'])

# Ajuster la taille du graphique
width = 1200
height = 800
graphique = (gf.coastline * points).opts(width=width, height=height)

# Définir un fichier de sortie pour le graphique
output_file("map_with_points.html", title="Map with Points")

# Créer le graphique
plot = gv.render(graphique)

# Afficher le graphique avec style pour le centrage
show(plot)

```

<img width="1204" alt="image" src="https://github.com/Gogo-IGM-BK/Python-Data/assets/73750131/a1c9e6f7-b7b4-4d62-b31d-01613ed22769">

