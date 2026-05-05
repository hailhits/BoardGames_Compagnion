# Game Night Rescue

**Game Night Rescue** est une PWA hors-ligne pour sauver les soirées de jeux quand il manque des morceaux : dés, argent, pions, papier, crayon, timer, feuilles de score ou idées de mini-jeux.

## Objectif du produit

- Fonctionne sur téléphone et tablette.
- Pensé pour un chalet, une soirée de famille, une coupure internet ou une vieille boîte de jeu incomplète.
- Aucun serveur obligatoire.
- Données sauvegardées localement dans le navigateur.
- Version gratuite avec contenu limité.
- Version Pro vendable avec Lemon Squeezy.

## Contenu gratuit inclus

1. Banque & Propriétés
2. 5 Dés & Feuille de score
3. Mot Mystère
4. X contre O
5. Défi de Dés

## Contenu Pro prévu

- Presets premium
- Mini-jeux premium
- Thèmes visuels premium
- Banque avancée
- Tournoi
- Cartes maison
- Créateur de jeu rapide Pro
- Export avancé

## Installation locale

```bash
npm install
npm run dev
```

## Build

```bash
npm run build
```

Le dossier généré est `dist/`.

## Déploiement Vercel

Réglages recommandés :

- Framework: Vite
- Install Command: `npm install`
- Build Command: `npm run build`
- Output Directory: `dist`

Le fichier `vercel.json` contient déjà ces réglages.

## Où changer les prix et le lien Lemon Squeezy

Ouvre :

```txt
src/config/monetization.js
```

Change :

```js
checkoutUrl: "https://example.com/checkout"
```

Tu peux aussi changer les prix affichés dans l'app.

## Où changer les jeux gratuits/payants

Ouvre :

```txt
src/data/gamePresets.js
```

Chaque preset contient :

```js
isFree: true
```

ou :

```js
isFree: false
```

## Où changer le style visuel

Ouvre :

```txt
src/styles/theme.css
src/styles/layout.css
src/styles/components.css
```

## Notes légales importantes

Cette app doit éviter de copier les noms officiels, logos officiels, images officielles, règles complètes ou contenus protégés de jeux existants.

Utilise des noms génériques comme :

- Banque & Propriétés
- 5 Dés & Feuille de score
- Ressources & Colonies
- Guerre de Territoires
- Carnet de Détective

## Structure du projet

Voir `MOBILE_GITHUB_STEPS.md` pour les étapes sur tablette Samsung.
