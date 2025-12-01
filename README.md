# 👋 Bonjour — Je suis Alexs Kapene

> *README de profil GitHub — propre, compatible GitHub, dark mode, fonctionnalités optimisées*

<p align="center">
  <img src="https://readme-typing-svg.herokuapp.com?font=Fira+Code&size=24&pause=2000&color=00FFD1&center=true&vCenter=true&width=650&lines=Développeur+Web+%7C+JavaScript+%7C+React+%7C+Flutter" />
</p>

---

## 🌑 Mode Sombre (Dark Mode)

GitHub active automatiquement le thème foncé du README si votre interface est en **Dark Mode**. Le README ci-dessous est optimisé pour bien s’afficher dans les deux thèmes.

---

## 💡 À propos de moi

Développeur web passionné, j'aime créer des interfaces modernes et performantes. Je travaille actuellement sur plusieurs projets frontend et mobile.

* 🌱 Technologies en cours d'apprentissage : **JavaScript, React, Flutter, NestJS, Git, GitHub Actions**.
* 🚀 Objectif : devenir développeur polyvalent (Frontend + Mobile + CI/CD).
* 🛠️ Toujours en amélioration continue.

---

## ⚡ Compétences principales

### 🔤 Langages

* HTML5
* CSS3
* JavaScript (ES6+)
* Dart (Flutter)

### 🧩 Frameworks & Libraries

* React
* Flutter
* NestJS
* TailwindCSS
* Bootstrap

### 🛠️ Outils & Plateformes

* Git & GitHub
* GitHub Actions (Automatisations CI/CD)
* GitHub Pages
* VS Code

---

## 🏅 Badges dynamiques

<p align="left">
  <img src="https://img.shields.io/github/followers/alexsKapene?label=Followers&style=for-the-badge" />
  <img src="https://github-readme-stats.vercel.app/api?username=alexsKapene&show_icons=true&theme=tokyonight" />
  <img src="https://github-readme-streak-stats.herokuapp.com/?user=alexsKapene&theme=tokyonight" />
</p>

---

## 🧩 Animations & Widgets GitHub

### ⭐ Stats globales

```md
![Stats GitHub](https://github-readme-stats.vercel.app/api?username=alexsKapene&show_icons=true&theme=tokyonight)
```

### 📊 Langages les plus utilisés

```md
![Top Langs](https://github-readme-stats.vercel.app/api/top-langs/?username=alexsKapene&layout=compact&theme=tokyonight)
```

### 🔁 Activité récente (automatisable)

```md
![GitHub Activity Graph](https://github-readme-activity-graph.vercel.app/graph?username=alexsKapene&theme=tokyonight)
```

---

## 🤖 Automatisations recommandées (GitHub Actions)

### CI standard pour React / Node

```yaml
name: CI
on:
  push:
    branches: [ main, dev ]
  pull_request:
    branches: [ main ]

jobs:
  build:
    runs-on: ubuntu-latest
    steps:
      - uses: actions/checkout@v4
      - uses: actions/setup-node@v4
        with:
          node-version: 18
      - run: npm ci
      - run: npm run build --if-present
      - run: npm test --if-present
```

### Déploiement GitHub Pages

```yaml
name: Deploy
on:
  push:
    branches: [ main ]

jobs:
  deploy:
    runs-on: ubuntu-latest
    steps:
      - uses: actions/checkout@v4
      - uses: actions/setup-node@v4
        with:
          node-version: 18
      - run: npm ci
      - run: npm run build
      - uses: peaceiris/actions-gh-pages@v3
        with:
          github_token: ${{ secrets.GITHUB_TOKEN }}
          publish_dir: ./build
```

### Mise à jour automatique du README

```yaml
name: Update README
on:
  schedule:
    - cron: "0 */12 * * *"
  workflow_dispatch:

jobs:
  update-readme:
    runs-on: ubuntu-latest
    steps:
      - uses: actions/checkout@v4
      - name: Auto-update
        run: |
          echo "Auto Update Triggered"
      - name: Push changes
        run: |
          git config user.name "github-actions[bot]"
          git config user.email "41898282+github-actions[bot]@users.noreply.github.com"
          git add .
          git commit -m "Auto update README" || exit 0
          git push
```

---

## 📦 Projets recommandés à mettre en avant

* **Portfolio** – HTML / CSS / JS
* **E-commerce Demo** – React & Bootstrap
* **Flutter App Demo** – Interface mobile
* **API NestJS** – Backend rapide et structuré

---

## 📬 Contact

* Ouvrez une **issue** avant de proposer des modifications.
* Suivez les standards : formatage, conventions de commits, branches claires.

---

*Fait avec ⚡, automatisations & Dark Mode*
