# Guide GitHub 🐱‍💻

GitHub est une plateforme de développement qui facilite la collaboration sur des projets. Voici un guide rapide pour gérer vos projets avec GitHub.

## 1. Configuration initiale 🛠️

Avant de commencer, assurez-vous d'avoir [installé Git](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git) sur votre machine.

1. Configurez votre nom d'utilisateur :

```
git config --global user.name "Votre nom"
```
2. Configurez votre adresse e-mail :

```
git config --global user.email "votre.email@exemple.com"
```

## 2. Créer un nouveau dépôt (repository) 📘

1. Allez sur [GitHub](https://github.com/).
2. Cliquez sur le bouton `+` en haut à droite et choisissez "New repository".
3. Suivez les étapes pour initialiser votre dépôt.

## 3. Cloner un dépôt existant 🚀

Pour travailler sur un projet existant depuis GitHub sur votre machine locale :
```
git clone lien_du_dépôt.git
```
## 4. Cycle de travail typique 🔄

1. **Pull** (Tirer) les dernières modifications :
```
git pull origin nom_de_la_branche
```
2. Apportez vos modifications au code.
3. **Add** (Ajouter) les fichiers modifiés :
```
   git add .
```
Ou, pour ajouter des fichiers spécifiques :
```
   git add nom_du_fichier
```
4. **Commit** (Valider) vos modifications :
```
git commit -m "Description des changements"
```
5. **Push** (Envoyer) vos modifications sur GitHub :
```
git push origin nom_de_la_branche
```

## 5. Branches et Pull Requests 🌿

- **Créer une nouvelle branche** :
```
git checkout -b nom_de_la_nouvelle_branche
```
- **Changer de branche** :
```
git checkout nom_de_la_branche
```
- Lorsque vous avez terminé votre travail sur une branche, créez une **Pull Request** sur GitHub pour proposer vos modifications à la branche principale.

## 6. Gérer les conflits ❗

Si vous avez des conflits entre votre code et la version actuelle du dépôt, Git vous informera lors d'un `pull` ou `push`. Résolvez les conflits manuellement en éditant les fichiers concernés, puis `add`, `commit` et `push` à nouveau.

> 📌 Astuce : Utilisez des outils comme [GitHub Desktop](https://desktop.github.com/) ou des extensions pour votre IDE pour gérer Git plus facilement.


