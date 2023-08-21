## 🌍 GeoViews 

GeoViews est une bibliothèque Python qui facilite la création de visualisations géospatiales interactives. Contrairement aux outils de visualisation géospatiale traditionnels, GeoViews est conçu pour fonctionner de manière transparente avec les structures de données multidimensionnelles de HoloViews, particulièrement celles de xarray.

### 📘 Résumé :

- 🖼 **Graphiques Géospatiaux**:

  GeoViews prend en charge de nombreux types de données géospatiales pour la visualisation, y compris les raster, les contours, les points, les lignes, les polygones et les vecteurs.
  
- 🔗 **Intégration avec d'autres bibliothèques**:

  Se combine parfaitement avec d'autres outils comme HoloViews, Bokeh et CartoPy pour créer des visualisations interactives avancées.

- 🔄 **Interactivité**:

  Profitez des widgets intégrés pour explorer dynamiquement les données géospatiales multidimensionnelles.

- 🌐 **Projections**:

  Changez facilement entre différentes projections cartographiques sans avoir à retraiter vos données.

- 🎨 **Personnalisation**:

  Tout comme avec HoloViews et Bokeh, vous pouvez personnaliser la présentation, le style, et la dynamique de vos visualisations.

### 🚀 Exemples d'utilisation :

1. **Visualisation d'un raster**:
```python
import geoviews as gv
import geoviews.feature as gf
import xarray as xr

ds = xr.tutorial.open_dataset('air_temperature').isel(time=0)
air_temp = gv.Dataset(ds).to(gv.Image, ['lon', 'lat'], 'air')
air_temp * gf.coastline
```
2. 🗺 **Affichage de points géospatiaux**:
```python
import numpy as np
points = gv.Points((np.random.rand(100), np.random.rand(100)))
points * gf.borders
```

3.🔍 **Carte interactive avec des tuiles**:
```python
gv.tile_sources.Wikipedia * gf.borders
```
