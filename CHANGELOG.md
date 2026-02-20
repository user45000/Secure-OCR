# Changelog

## v2.2.3 (2025-02-19)
- Indicateur "Données anonymisées avant envoi" à côté du bouton Corriger

## v2.2.2 (2025-02-19)
- Le texte collé passe par `cleanText()` (suppression retours à la ligne, nettoyage espaces)

## v2.2.1 (2025-02-19)
- Fix affichage du texte collé (placeholder, contentEditable, compteur)

## v2.2.0 (2025-02-19)
- **Mode texte direct** : bouton "Coller du texte" dans la dropzone
- **Ctrl+V intelligent** : détecte image vs texte dans le presse-papier
- Panneau d'info "Texte collé" avec statistiques

## v2.1.4 (2025-02-19)
- Fix anonymisation : "En" de "En effet" capturé après Mr (Pattern C → trimName)
- Ajout pattern RPPS/ADELI/FINESS avant téléphone
- Ajout person markers : patient(e), requérant(e), expert(e)
- Nouveau pattern standalone `Prénom NOM` (NOM ≥3 majuscules)
- Nouveau pattern contextuel `Nom, remplaçant(e)/interne`

## v2.1.3 (2025-02-19)
- Bouton Copier unifié déplacé dans le header, icône SVG

## v2.1.2 (2025-02-19)
- Bouton Copier unifié (fusion "Tout" / "Page"), feedback animé

## v2.1.1 (2025-02-19)
- Fix sélection canvas décalée (CSS canvas-area/canvas-inner)
- Fix panneau réglages (position fixed, pointer-events SVG, click-outside)

## v2.1.0 (2025-02-19)
- **Refonte design complète** : nouvelle palette bleu/vert, Plus Jakarta Sans
- Topbar simplifiée : réglages dans panneau ⚙️ rétractable
- Logo bouclier SVG, dropzone redessinée avec border dashed
- Badge sécurité "🛡 Anonymisé" dans la topbar
- Mention "Traitement local" dans la dropzone
- Texte résultat en sans-serif pour meilleure lisibilité

## v2.0.3 (2025-02-19)
- Réécriture complète de l'anonymisation
- Fix faux positifs : mots communs français, titres de personnes
- Fix captures manquées : astérisques, labels médicaux, deux-points intermédiaires
- Validation `isValidName`, `trimName`, `isCommonWord`
- 30 cas de test, 100% pass

## v2.0.2 (2025-02-19)
- Réécriture regex NIR/SSN
- Expansion des marqueurs de champs et stop-words
- Renommage en "Secure OCR"

## v2.0.1 (2025-02-18)
- Bouton sauvegarder, diff inline, toggle auto-correct

## v2.0.0 (2025-02-18)
- Intégration Mistral AI pour correction OCR
- Anonymisation / dé-anonymisation des données médicales
- Gestion clé API via localStorage

## v1.0.0 (2025-02-16)
- OCR navigateur avec Tesseract.js
- Support PDF multi-pages avec sidebar
- Sélection de zone, thème sombre
- Zones turquoise persistantes
