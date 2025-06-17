# Commandes BASH

## Navigation dans le système de fichiers

| Commande | Description                             |
| -------- | --------------------------------------- |
| `pwd`    | Affiche le chemin du répertoire courant |
| `ls`     | Liste les fichiers/répertoires          |
| `cd`     | Change de répertoire                    |
| `cd ..`  | Remonte d’un niveau dans l’arborescence |
| `cd ~`   | Va dans le répertoire personnel         |
| `tree`   | Affiche l’arborescence des fichiers     |

## Manipulation de fichiers et de répertoires

| Commande            | Description                           |
| ------------------- | ------------------------------------- |
| `touch fichier.txt` | Crée un fichier vide                  |
| `mkdir mon_dossier` | Crée un dossier                       |
| `cp source dest`    | Copie un fichier ou un dossier        |
| `mv source dest`    | Déplace ou renomme un fichier/dossier |
| `rm fichier.txt`    | Supprime un fichier                   |
| `rm -r dossier`     | Supprime un dossier et son contenu    |

## Visualisation et recherche

| Commande                       | Description                             |
| ------------------------------ | --------------------------------------- |
| `cat fichier.txt`              | Affiche le contenu d’un fichier         |
| `less fichier.txt`             | Affiche avec navigation (page par page) |
| `head -n 10 fichier.txt`       | Affiche les 10 premières lignes         |
| `tail -n 10 fichier.txt`       | Affiche les 10 dernières lignes         |
| `grep "mot" fichier.txt`       | Cherche une chaîne dans un fichier      |
| `find /chemin -name "fichier"` | Recherche un fichier par nom            |

## Utilitaires système

| Commande       | Description                      |
| -------------- | -------------------------------- |
| `man commande` | Affiche le manuel de la commande |
| `chmod`        | Modifie les permissions          |
| `chown`        | Change le propriétaire           |
| `top` / `htop` | Affiche les processus en cours   |
| `ps`           | Liste les processus en cours     |
| `kill PID`     | Termine un processus par son ID  |

## Archivage et compression

| Commande                          | Description                |
| --------------------------------- | -------------------------- |
| `tar -czf archive.tar.gz dossier` | Compresse un dossier       |
| `tar -xzf archive.tar.gz`         | Décompresse une archive    |
| `zip archive.zip fichier`         | Crée un fichier zip        |
| `unzip archive.zip`               | Décompresse un fichier zip |

## Réseau

| Commande             | Description                          |
| -------------------- | ------------------------------------ |
| `ping adresse`       | Teste la connectivité réseau         |
| `curl url`           | Télécharge du contenu depuis une URL |
| `wget url`           | Autre outil de téléchargement        |
| `ifconfig` ou `ip a` | Affiche les interfaces réseau        |

## Commandes avancées et scripts

| Commande         | Description                                         |                                                       |
| ---------------- | --------------------------------------------------- | ----------------------------------------------------- |
| `echo "texte"`   | Affiche du texte                                    |                                                       |
| `>` et `>>`      | Redirection de sortie (écrase ou ajoute)            |                                                       |
| \`               | \`                                                  | Pipe : envoie la sortie d'une commande vers une autre |
| `&&`             | Exécute la commande suivante si la première réussit |                                                       |
| `;`              | Enchaîne les commandes                              |                                                       |
| `bash script.sh` | Exécute un script Bash                              |                                                       |

```js
console.log("Hello World);
```