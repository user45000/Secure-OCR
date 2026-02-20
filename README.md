# 🛡️ Secure OCR

**Extracteur de texte sécurisé avec anonymisation médicale et correction IA.**

Secure OCR est un outil 100% client-side (HTML/JS) qui permet d'extraire du texte depuis des images et PDF, de l'anonymiser automatiquement (noms, NIR, dates, adresses, RPPS...) et de le corriger via IA — le tout sans qu'aucune donnée personnelle ne quitte votre machine.

## ✨ Fonctionnalités

- **OCR navigateur** — Tesseract.js, 13 langues supportées, sélection de zone
- **Mode texte direct** — Collez du texte depuis n'importe quelle source (Ctrl+V)
- **Anonymisation automatique** — 14 types de données sensibles détectés (NIR, noms, dates, téléphones, RPPS, adresses...)
- **Correction IA** — Mistral AI corrige les erreurs OCR sur le texte anonymisé
- **Dé-anonymisation** — Les données originales sont restaurées après correction
- **PDF multi-pages** — Sidebar avec miniatures, navigation, extraction par lot
- **100% local** — Aucun serveur, aucune base de données, aucun cookie

## 🔒 Sécurité

L'anonymisation se fait **avant** tout envoi réseau. Le texte transmis à Mistral ne contient que des marqueurs (`[NOM_1]`, `[NIR_2]`, `[DATE_3]`...). Les données originales restent dans le navigateur et sont restaurées après correction.

## 🚀 Utilisation

### En ligne
👉 **[Lancer Secure OCR](https://VOTRE-USERNAME.github.io/secure-ocr/)**

### En local
1. Téléchargez `index.html`
2. Ouvrez-le dans votre navigateur
3. C'est tout — aucune installation requise

### Correction IA (optionnel)
1. Créez un compte gratuit sur [console.mistral.ai](https://console.mistral.ai) (plan Experiment, sans CB)
2. Générez une clé API
3. Cliquez 🔑 dans Secure OCR et collez votre clé

## 📋 Changelog

Voir [CHANGELOG.md](CHANGELOG.md)

## 📄 Licence

Ce projet est distribué sous licence MIT. Voir [LICENSE](LICENSE).
