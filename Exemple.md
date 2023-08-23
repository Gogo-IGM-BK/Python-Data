# 1. 📊 Distribution Plot (simple):

C'est un outil pour visualiser la distribution d'une variable sous forme d'histogramme.
```python
import seaborn as sns
import matplotlib.pyplot as plt

# Données
data = sns.load_dataset("iris")

# Création d'un graphique de distribution pour la caractéristique "sepal_length"
sns.distplot(data["sepal_length"], bins=20, kde=True, color="skyblue")
plt.title("Distribution de la longueur du sépale")
plt.show()

```
# 2. 📈 Box Plot avec Hue (plus avancé):
Il permet de visualiser la distribution d'une variable catégorique, en montrant des informations comme la médiane, les quartiles et les valeurs aberrantes.
```python
import seaborn as sns
import matplotlib.pyplot as plt

# Données
data = sns.load_dataset("tips")

# Création d'un box plot pour visualiser la distribution des factures totales par jour et par sexe.
sns.boxplot(x="day", y="total_bill", hue="sex", data=data, palette="coolwarm")
plt.title("Distribution des factures totales par jour et par sexe")
plt.show()

```
# 3. 🌐 FacetGrid avec scatter plot (plus avancé):

FacetGrid est un outil pour visualiser la distribution de plusieurs variables à la fois, par rapport à une ou deux variables catégorielles.

```python
import seaborn as sns
import matplotlib.pyplot as plt

# Données
data = sns.load_dataset("tips")

# Création d'une grille de nuages de points pour visualiser le rapport entre la facture totale et le pourboire, divisé par le moment (déjeuner/dîner) et le sexe.
g = sns.FacetGrid(data, col="time", row="sex", margin_titles=True)
g.map(plt.scatter, "total_bill", "tip", edgecolor="w")
g.fig.subplots_adjust(wspace=0, hspace=0)

# Affichage des titres
g.fig.suptitle("Relation entre le total de la facture et le pourboire, par sexe et moment", y=1.02)
plt.show()

```




