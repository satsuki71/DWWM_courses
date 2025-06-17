# 📁 Structuration Complète d’un Projet Web

---

## 1. Structure de dossier recommandée

```
mon-projet-web
├── public/ # Fichiers statiques accessibles (HTML, favicon, robots.txt)
│ ├── index.html # Page d’accueil principale
│ ├── about.html # Exemple d’autres pages HTML
│ ├── favicon.ico # Icône du site
│ └── assets/ # Images, vidéos, polices, etc.
│ ├── img/
│ ├── fonts/
│ └── videos/
├── src/ # Code source (JS, CSS, etc.)
│ ├── css/ # Feuilles de style
│ │ └── styles.css
│ ├── js/ # Scripts JavaScript
│ │ └── main.js
│ └── components/ # (si projet avec composants réutilisables)
├── tests/ # Tests unitaires ou fonctionnels
├── docs/ # Documentation technique ou utilisateur
├── .gitignore # Fichiers/dossiers ignorés par Git
├── package.json # Configuration du projet (npm, dépendances, scripts)
├── README.md # Documentation générale du projet
└── webpack.config.js # (si utilisation de bundler comme Webpack)
```

---

## 2. Description détaillée des dossiers/fichiers

| Élément             | Description                                               | Exemple / Notes                                |
|---------------------|-----------------------------------------------------------|-----------------------------------------------|
| `public/`           | Contient les fichiers accessibles directement via URL    | HTML, favicon, fichiers statiques             |
| `src/`              | Contient le code source à compiler ou bundler             | JS, CSS, composants, modules                   |
| `src/css/`          | Styles CSS                                                | `styles.css`, fichiers SCSS/SASS si utilisé   |
| `src/js/`           | Scripts JavaScript                                        | `main.js`, modules, utilitaires                |
| `src/components/`   | Composants réutilisables (React, Vue, etc.)              | Pour une architecture modulaire                |
| `tests/`            | Tests automatisés                                        | Jest, Mocha, Cypress, etc.                      |
| `docs/`             | Documentation du projet                                  | Guides utilisateurs, spécifications             |
| `.gitignore`        | Liste des fichiers à ignorer dans le dépôt Git            | `node_modules/`, fichiers build, secrets       |
| `package.json`      | Gestionnaire de dépendances et scripts (npm, yarn)        | Scripts de build, start, test                   |
| `README.md`         | Présentation et instructions du projet                    | Important pour la compréhension globale         |
| `webpack.config.js` | Configuration du bundler (optionnel)                      | Pour projets avec bundling JavaScript           |

---

## 3. Exemple simple de fichiers clés

### a) `public/index.html`

```html
<!DOCTYPE html>
<html lang="fr">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Mon Projet Web</title>
  <link rel="stylesheet" href="../src/css/styles.css" />
</head>
<body>
  <h1>Bienvenue sur mon site</h1>
  <script src="../src/js/main.js"></script>
</body>
</html>
```

### b) src/css/styles.css
```css
body {
  font-family: Arial, sans-serif;
  margin: 0;
  padding: 0;
  background-color: #f5f5f5;
}
h1 {
  color: #333;
  text-align: center;
  margin-top: 2rem;
}
```

### c) src/js/main.js

```js
document.addEventListener('DOMContentLoaded', () => {
  console.log('Bienvenue dans mon projet web!');
});
```

## 4. Bonnes pratiques supplémentaires
- Séparer le code métier (JS) du style (CSS) et de la structure (HTML) pour plus de clarté

- Utiliser un gestionnaire de dépendances (npm ou yarn) même pour projets simples, ça facilite l’ajout de bibliothèques

- Mettre en place un .gitignore adapté (exemple minimal : node_modules/, dist/, .env)

- Écrire un README.md clair pour expliquer l’installation, l’usage et la contribution

- Structurer les composants si tu utilises un framework front (React, Vue) pour modulariser

- Ajouter des tests dans un dossier tests/ pour la qualité du code

- Utiliser un bundler (Webpack, Vite) si tu as plusieurs fichiers JS/CSS pour optimiser et gérer les dépendances

## 5. Exemple minimal .gitignore

```
node_modules/
dist/
.env
.DS_Store
*.log
```

## 6. Exemples d’outils à intégrer

| Outil                     | Usage                                             |
| --------------------------- | ------------------------------------------------------- |
| Webpack / Vite                | Bundler JS/CSS                  |
| Babel                | Transpileur JS moderne vers compatible    |
| ESLint               | Linter pour garder un code propre      |
| Prettier                | Formatteur de code                         |
| Jest / Mocha                   | Tests unitaires                 |

## 7. Fichiers courants dans un projet web

| Fichier                     | Description                                             |
| --------------------------- | ------------------------------------------------------- |
| `index.html`                | Page d’accueil principale du site web                   |
| `about.html`                | Exemple de page supplémentaire (ex: page "À propos")    |
| `favicon.ico`               | Icône du site affichée dans l’onglet du navigateur      |
| `styles.css`                | Fichier principal de styles CSS                         |
| `main.js`                   | Fichier principal de scripts JavaScript                 |
| `package.json`              | Configuration du projet (dépendances, scripts npm/yarn) |
| `.gitignore`                | Liste des fichiers et dossiers à ignorer dans Git       |
| `README.md`                 | Documentation générale du projet                        |
| `.env`                      | Variables d’environnement (clés API, configs sensibles) |
| `webpack.config.js`         | Configuration du bundler Webpack (si utilisé)           |
| `babel.config.js`           | Configuration du transpileur Babel (si utilisé)         |
| `LICENSE`                   | Licence du projet (ex: MIT, GPL)                        |
| `robots.txt`                | Instructions pour les moteurs de recherche              |
| `manifest.json`             | Configuration pour les Progressive Web Apps (PWA)       |
| `tsconfig.json`             | Configuration TypeScript (si utilisé)                   |
| `eslint.json` / `.eslintrc` | Configuration du linter ESLint                          |
| `.prettierrc`               | Configuration du formateur de code Prettier             |
| `tests/`                    | Dossier contenant les tests (unitaires, d’intégration)  |
| `docs/`                     | Dossier de documentation technique ou utilisateur       |
