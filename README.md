# 🧩 Programmation Orientée Objet avec Python

## 🏫 Classes et Objets

En Python, une classe est comme un plan pour créer des objets. Un objet est une instance d'une classe.

```python
class MaClasse:
    x = 5

mon_objet = MaClasse()
print(mon_objet.x)  # affiche 5
```
## ⬆️ Héritage
L'héritage permet de définir une classe qui hérite de toutes les méthodes et propriétés d'une autre classe.

```python
class Personne:
  def saluer(self):
    print("Bonjour!")

class Etudiant(Personne):
  pass

etudiant = Etudiant()
etudiant.saluer()  # affiche "Bonjour!"

```

## 📦 Encapsulation
L'encapsulation en Python est la restriction de l'accès aux méthodes et aux variables d'une classe. Cela peut être accompli en utilisant des méthodes privées et des propriétés.

```python
class Voiture:
  def __init__(self):
    self.__maxspeed = 200  # Ceci est une variable privée

  def conduire(self):
    print(f'Conduire à une vitesse maximale de {self.__maxspeed}')

voiture = Voiture()
voiture.conduire()

```

## 🔄 Polymorphisme
Le polymorphisme est un principe de POO qui permet à une classe d'être définie de plusieurs façons. En Python, le polymorphisme est implémenté à travers les méthodes.

```python
class Chien:
  def son(self):
    return "ouaf ouaf"

class Chat:
  def son(self):
    return "miaou"

def faire_du_bruit(animal):
  print(animal.son())

mon_chien = Chien()
mon_chat = Chat()

faire_du_bruit(mon_chien)  # affiche "ouaf ouaf"
faire_du_bruit(mon_chat)  # affiche "miaou"


```











