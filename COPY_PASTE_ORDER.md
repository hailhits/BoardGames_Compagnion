# Ordre conseillé pour créer les fichiers à la main

Si tu ne peux pas uploader les dossiers, crée les fichiers dans cet ordre.

## Bloc 1 — racine

1. `package.json`
2. `index.html`
3. `vite.config.js`
4. `vercel.json`
5. `.gitignore`
6. `README.md`
7. `MOBILE_GITHUB_STEPS.md`

## Bloc 2 — public

1. `public/manifest.webmanifest`
2. `public/sw.js`
3. `public/assets/app-icon.svg`

## Bloc 3 — src base

1. `src/main.jsx`
2. `src/App.jsx`
3. `src/config/monetization.js`
4. `src/context/AppContext.jsx`

## Bloc 4 — data / hooks / utils

1. `src/data/defaultState.js`
2. `src/data/gamePresets.js`
3. `src/data/quickWords.js`
4. `src/data/themes.js`
5. `src/hooks/useLocalStorage.js`
6. `src/hooks/useTimer.js`
7. `src/utils/access.js`
8. `src/utils/dice.js`
9. `src/utils/exportImport.js`
10. `src/utils/format.js`
11. `src/utils/id.js`
12. `src/utils/storage.js`

## Bloc 5 — layout / components

1. `src/layout/AppShell.jsx`
2. `src/layout/BottomNav.jsx`
3. `src/layout/Header.jsx`
4. `src/layout/PageTitle.jsx`
5. `src/components/Button.jsx`
6. `src/components/Card.jsx`
7. `src/components/EmptyState.jsx`
8. `src/components/LockBadge.jsx`
9. `src/components/Modal.jsx`
10. `src/components/StatPill.jsx`

## Bloc 6 — features

Tous les fichiers dans `src/features/...`

## Bloc 7 — styles

1. `src/styles/index.css`
2. `src/styles/theme.css`
3. `src/styles/layout.css`
4. `src/styles/components.css`
