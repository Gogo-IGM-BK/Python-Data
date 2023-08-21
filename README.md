## 🎨 Seaborn

Seaborn est une bibliothèque de visualisation de données en Python basée sur Matplotlib. Elle offre une interface de haut niveau pour créer des graphiques statistiques attrayants et est particulièrement adaptée pour visualiser des dataframes de Pandas.

### 📘 Résumé :

- 🌈 **Thèmes et Styles**: Seaborn fournit des thèmes prédéfinis qui améliorent l'esthétique et la lisibilité des graphiques par rapport à Matplotlib.
- 📊 **Graphiques Statistiques**: Avec Seaborn, il est facile de créer des graphiques complexes tels que des matrices de corrélation, des graphiques en violon et des diagrammes en boîte.
- 💡 **Facilité d'utilisation**: Seaborn s'intègre parfaitement avec les DataFrames de Pandas, simplifiant la visualisation des données.
- 🎚 **Personnalisation**: Bien que Seaborn soit plus abstrait que Matplotlib, il offre toujours une grande personnalisation pour ceux qui souhaitent peaufiner leurs visualisations.
- 🌐 **Extension**: Utilise Matplotlib sous le capot, ce qui permet une combinaison fluide des fonctionnalités des deux bibliothèques.

### 🚀 Exemples d'utilisation :

1. **Diagramme en barres**:
```python
import seaborn as sns

tips = sns.load_dataset("tips")
sns.barplot(x="day", y="total_bill", data=tips)
```
2. **🎻 Graphique en violon**:
```python
sns.violinplot(x="day", y="total_bill", data=tips, palette="pastel")
```
3. **🔥 Carte thermique (heatmap)**:
```python
corr = tips.corr()
sns.heatmap(corr, annot=True, cmap="coolwarm")
```
4. **📦 Diagramme en boîte (box plot)**:
```python
sns.boxplot(x="day", y="total_bill", hue="sex", data=tips, palette="muted")
```
