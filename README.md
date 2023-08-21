# Gestion des Environnements Virtuels en Python 🐍

La gestion des environnements virtuels est une étape cruciale pour garantir l'isolation des dépendances de projet. Voici un guide rapide pour utiliser `venv` en Python.

## 1. Installer `venv` 📦

Pour commencer, installez le module `virtualenv`:
```python
pip install virtualenv
```

## 2. Création d'un environnement virtuel 🌍

- Ouvrez un terminal ou un invite de commande.
- Naviguez vers le répertoire où vous souhaitez créer votre environnement virtuel.
- Exécutez la commande suivante :

```python
python -m venv nom_de_l_environnement
```


## 3. Activer l'environnement virtuel 🚀

Activez votre environnement avec la commande :
```python
source nom_de_l_environnement/bin/activate
```


## 4. Installer des paquets 📚

Avec l'environnement virtuel activé, installez les paquets nécessaires avec `pip`:

```python
pip install nom_du_paquet
```

> 📌 Note: Les paquets installés dans cet environnement ne seront disponibles que là.

## 5. Désactiver l'environnement virtuel ❌

Lorsque vous avez terminé, désactivez l'environnement:

```python
deactivate
```


## 6. Supprimer l'environnement virtuel 🗑️

Si vous n'avez plus besoin de l'environnement :

1. Désactivez-le.
2. Supprimez le dossier associé:

```python
rm -r nom_de_l_environnement/
```


## 7. Gérer les dépendances 📄

### Créer un fichier `requirements.txt` 

Pour lister toutes les dépendances de votre projet :

```python
pip freeze > requirements.txt
```


### Installer des dépendances depuis `requirements.txt`

Pour installer toutes les dépendances listées dans le fichier :

```python
pip install -r requirements.txt
```







