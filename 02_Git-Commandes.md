# 🧠 Git – Principales Commandes

Un résumé clair et structuré des commandes Git les plus utilisées, organisé par thème.

---

## ⚙️ Configuration initiale

| Commande                                         | Description                                |
|--------------------------------------------------|--------------------------------------------|
| `git config --global user.name "Ton Nom"`        | Définit ton nom pour tous les dépôts       |
| `git config --global user.email "ton@email.com"` | Définit ton email pour tous les dépôts     |

---

## 🆕 Créer ou cloner un dépôt

| Commande                 | Description                                      |
|--------------------------|--------------------------------------------------|
| `git init`              | Initialise un dépôt Git local                    |
| `git clone <url>`       | Clone un dépôt distant sur ta machine            |

---

## 📂 Travailler avec les fichiers

| Commande                     | Description                                        |
|------------------------------|----------------------------------------------------|
| `git status`                 | Affiche les fichiers modifiés ou non suivis       |
| `git add <fichier>`          | Ajoute un fichier à l'index (staging)             |
| `git add .`                  | Ajoute tous les fichiers modifiés                 |
| `git commit -m "message"`    | Valide les changements avec un message            |

---

## 📖 Historique

| Commande                                | Description                                      |
|-----------------------------------------|--------------------------------------------------|
| `git log`                               | Affiche l'historique complet des commits         |
| `git log --oneline --graph --all`       | Historique résumé avec graphe de branches        |

---

## 🛠️ Modifier ou annuler des changements

| Commande                          | Description                                                     |
|-----------------------------------|-----------------------------------------------------------------|
| `git diff`                        | Montre les différences non indexées                             |
| `git checkout -- <fichier>`      | Annule les modifications locales d’un fichier                   |
| `git reset HEAD <fichier>`       | Retire un fichier de l’index sans supprimer ses modifications   |

---

## 🌿 Branches

| Commande                         | Description                                      |
|----------------------------------|--------------------------------------------------|
| `git branch`                     | Liste les branches                              |
| `git branch <nom>`              | Crée une nouvelle branche                        |
| `git checkout <branche>`         | Bascule vers une autre branche                  |
| `git switch <branche>`           | Bascule vers une autre branche (nouvelle syntaxe)|
| `git merge <branche>`            | Fusionne une branche dans celle en cours        |

---

## ⬆️ Travailler avec un dépôt distant

| Commande                                | Description                                              |
|-----------------------------------------|----------------------------------------------------------|
| `git remote add origin <url>`           | Lie le dépôt local à un dépôt distant (ex. GitHub)       |
| `git push origin <branche>`             | Envoie les commits vers le dépôt distant                 |
| `git pull`                              | Récupère et fusionne les changements du dépôt distant    |

---

## 🧹 Nettoyage

| Commande              | Description                                               |
|-----------------------|-----------------------------------------------------------|
| `git rm <fichier>`    | Supprime un fichier du projet et de Git                  |
| `git clean -fd`       | Supprime les fichiers/dossiers non suivis (⚠️ dangereux)  |

---

## 💡 Commandes utiles

| Commande                     | Description                                             |
|------------------------------|---------------------------------------------------------|
| `git stash`                  | Met de côté les modifications en cours                 |
| `git stash pop`              | Restaure les modifications mises de côté              |
| `git show <commit>`          | Affiche le contenu et les métadonnées d’un commit     |
| `git blame <fichier>`        | Affiche qui a modifié chaque ligne d’un fichier        |

---

## ✅ Bonnes pratiques

- 💬 Faire des messages de commit clairs et concis  
- 🌿 Travailler dans des branches (`feature/`, `fix/`, etc.)  
- 🔄 Toujours faire `git pull` avant un `git push`  
- 🚫 Utiliser un `.gitignore` adapté pour ignorer les fichiers inutiles  

---

## 🔗 Ressources utiles

- 📘 [Documentation Git officielle](https://git-scm.com/doc)  
- 📄 [Cheatsheet GitHub (PDF)](https://education.github.com/git-cheat-sheet-education.pdf)  
- 🎮 [Learn Git Branching (site interactif)](https://learngitbranching.js.org/)

---
