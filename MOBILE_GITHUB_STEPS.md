# Étapes GitHub sur tablette Samsung S6 Lite

Ce guide est fait pour créer le projet directement dans GitHub avec une tablette.

## Méthode recommandée

Tu as deux choix :

### Choix A — Upload fichier par fichier

1. Ouvre ton repository GitHub.
2. Crée les dossiers dans GitHub.
3. Entre dans chaque dossier.
4. Upload seulement les fichiers de ce dossier.

### Choix B — Copier-coller fichier par fichier

1. Ouvre ton repository GitHub.
2. Clique `Add file`.
3. Clique `Create new file`.
4. Dans le nom du fichier, écris le chemin complet, exemple :

```txt
src/main.jsx
```

GitHub va créer le dossier `src` automatiquement.

5. Copie-colle le contenu du fichier.
6. Clique `Commit changes`.

## Ordre le plus simple

### 1. Fichiers racine

À la racine du repo :

```txt
package.json
index.html
vite.config.js
vercel.json
.gitignore
README.md
MOBILE_GITHUB_STEPS.md
```

### 2. Dossier public

Créer :

```txt
public/manifest.webmanifest
public/sw.js
public/assets/app-icon.svg
```

### 3. Dossier src

Créer tous les fichiers `src/...` selon l'arbre du projet.

## Arbre complet

```txt
game-night-rescue/
├── README.md
├── MOBILE_GITHUB_STEPS.md
├── package.json
├── index.html
├── vite.config.js
├── vercel.json
├── .gitignore
├── public/
│   ├── manifest.webmanifest
│   ├── sw.js
│   └── assets/
│       └── app-icon.svg
└── src/
    ├── main.jsx
    ├── App.jsx
    ├── config/
    │   └── monetization.js
    ├── context/
    │   └── AppContext.jsx
    ├── data/
    │   ├── defaultState.js
    │   ├── gamePresets.js
    │   ├── quickWords.js
    │   └── themes.js
    ├── hooks/
    │   ├── useLocalStorage.js
    │   └── useTimer.js
    ├── utils/
    │   ├── access.js
    │   ├── dice.js
    │   ├── exportImport.js
    │   ├── format.js
    │   ├── id.js
    │   └── storage.js
    ├── layout/
    │   ├── AppShell.jsx
    │   ├── BottomNav.jsx
    │   ├── Header.jsx
    │   └── PageTitle.jsx
    ├── components/
    │   ├── Button.jsx
    │   ├── Card.jsx
    │   ├── EmptyState.jsx
    │   ├── LockBadge.jsx
    │   ├── Modal.jsx
    │   └── StatPill.jsx
    ├── features/
    │   ├── bank/
    │   │   ├── BankPage.jsx
    │   │   ├── PlayerMoneyCard.jsx
    │   │   └── TransactionForm.jsx
    │   ├── history/
    │   │   └── HistoryPage.jsx
    │   ├── home/
    │   │   └── HomePage.jsx
    │   ├── library/
    │   │   ├── LibraryPage.jsx
    │   │   └── PresetCard.jsx
    │   ├── minigames/
    │   │   ├── DiceChallengeGame.jsx
    │   │   ├── HangmanGame.jsx
    │   │   ├── MiniGamesPage.jsx
    │   │   └── TicTacToeGame.jsx
    │   ├── rescue/
    │   │   └── RescueWizard.jsx
    │   ├── settings/
    │   │   └── SettingsPage.jsx
    │   ├── tools/
    │   │   ├── CounterTool.jsx
    │   │   ├── DiceTool.jsx
    │   │   ├── NotesTool.jsx
    │   │   ├── RandomPickerTool.jsx
    │   │   ├── ScoreboardTool.jsx
    │   │   ├── TimerTool.jsx
    │   │   └── ToolsPage.jsx
    │   └── upgrade/
    │       └── UpgradePage.jsx
    └── styles/
        ├── components.css
        ├── index.css
        ├── layout.css
        └── theme.css
```

## Après avoir créé les fichiers

1. Va dans Vercel.
2. Add New Project.
3. Sélectionne ton repo GitHub.
4. Framework: Vite.
5. Build command: `npm run build`.
6. Output directory: `dist`.
7. Deploy.

## Si tu as une page blanche

Vérifie en premier :

1. `src/main.jsx` existe.
2. `src/App.jsx` existe.
3. `index.html` pointe vers `/src/main.jsx`.
4. Le fichier `package.json` est à la racine.
5. Dans Vercel, le build command est `npm run build`.
6. Dans Vercel, output directory est `dist`.
