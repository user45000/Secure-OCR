# 🚀 Mise en place GitHub — Guide pas à pas

## 1. Créer un compte GitHub (si pas déjà fait)

→ https://github.com/signup (gratuit)

## 2. Installer Git sur ton PC

→ https://git-scm.com/download/win

Pendant l'installation, garde toutes les options par défaut.

## 3. Créer le repo sur GitHub

1. Va sur https://github.com/new
2. **Repository name** : `secure-ocr`
3. **Description** : `Extracteur de texte sécurisé avec anonymisation médicale et correction IA`
4. **Public** (pour GitHub Pages gratuit) ou **Private** (si tu veux garder le code privé — GitHub Pages nécessite un plan Pro pour les repos privés)
5. **NE COCHE RIEN** (pas de README, pas de .gitignore, pas de licence — on a déjà tout)
6. Clique **Create repository**

## 4. Préparer le dossier local

Crée un dossier `secure-ocr` quelque part sur ton PC et mets-y les fichiers du repo :

```
secure-ocr/
├── index.html          ← le fichier secure-ocr.html renommé
├── README.md
├── CHANGELOG.md
├── LICENSE
└── .gitignore
```

## 5. Initialiser Git et pousser

Ouvre un terminal (clic droit → "Git Bash Here" dans le dossier secure-ocr) :

```bash
git init
git add .
git commit -m "v2.2.3 — Secure OCR initial release"
git branch -M main
git remote add origin https://github.com/user45000/secure-ocr.git
git push -u origin main
```

Remplace `user45000` par ton nom d'utilisateur GitHub.

## 6. Activer GitHub Pages

1. Va sur ton repo : `https://github.com/user45000/secure-ocr`
2. **Settings** → **Pages** (dans le menu de gauche)
3. **Source** : `Deploy from a branch`
4. **Branch** : `main` / `/ (root)`
5. Clique **Save**
6. Attends 1-2 minutes

→ Ton outil est maintenant accessible sur : **`https://user45000.github.io/secure-ocr/`**

## 7. Workflow quotidien

À chaque nouvelle version, tu mets à jour `index.html` dans le dossier puis :

```bash
git add .
git commit -m "v2.2.4 — Description du changement"
git push
```

Le site se met à jour automatiquement en ~30 secondes.

## Bonus : créer un tag pour chaque version

```bash
git tag v2.2.3
git push --tags
```

Les tags apparaissent dans l'onglet "Releases" sur GitHub et permettent de retrouver n'importe quelle version.
