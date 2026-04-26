# Pokémon Tracker FR — PWA Mobile

Suivi de prix de cartes Pokémon françaises, optimisé Android.

## Déploiement GitHub Pages (gratuit, 5 minutes)

### Étape 1 — Créer un compte GitHub
→ https://github.com/signup (gratuit)

### Étape 2 — Créer un nouveau dépôt
1. Clique sur "+" → "New repository"
2. Nom : `pokemon-tracker` (ou ce que tu veux)
3. Coche "Public"
4. Clique "Create repository"

### Étape 3 — Uploader les fichiers
1. Sur la page du dépôt, clique "uploading an existing file"
2. Glisse-dépose TOUS les fichiers (index.html, sw.js, manifest.json, et le dossier icons/)
3. Clique "Commit changes"

### Étape 4 — Activer GitHub Pages
1. Va dans "Settings" du dépôt
2. Menu gauche → "Pages"
3. Source : "Deploy from a branch"
4. Branch : "main" / "(root)"
5. Clique "Save"

### Étape 5 — Installer sur Android
1. Ouvre Chrome sur ton téléphone
2. Va sur : `https://TON_PSEUDO.github.io/pokemon-tracker`
3. Chrome affiche une bannière "Ajouter à l'écran d'accueil" → Accepte
4. L'app apparaît comme une vraie appli sur ton écran !

## Fichiers
- `index.html` — App principale
- `sw.js` — Service Worker (mode hors-ligne)
- `manifest.json` — Métadonnées PWA
- `icons/` — Icônes app

## Données
Toutes tes cartes et l'historique sont sauvegardés dans le localStorage du téléphone.
Ils survivent aux redémarrages mais PAS à une désinstallation / vidage du cache Chrome.
→ Pense à faire un export JSON de temps en temps (feature à venir).

## Quota API
- Max 4 lots/semaine (lots de 10 cartes)
- ~3% du quota gratuit Claude
- Les cartes les plus chères sont mises à jour en priorité
