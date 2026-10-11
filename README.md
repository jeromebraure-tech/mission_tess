# Mission Tess
Jeu de multiplication en français, sans dépendances, pour téléphone et ordinateur.

## Mettre en ligne sur GitHub Pages
1. Créer un dépôt public nommé `mission-tess` sur votre GitHub.
2. Décompresser l’archive et envoyer le CONTENU du dossier dans le dépôt : `index.html`, `sw.js`, `manifest.webmanifest`, les deux icônes et ce README. index.html doit être à la racine.
3. Dans Settings → Pages → Build and deployment, choisir Deploy from a branch, puis `main` et `/ (root)`. Enregistrer.
4. Attendre la publication. Le lien sera `https://VOTRE-PSEUDO.github.io/mission-tess/` (remplacer VOTRE-PSEUDO).
5. Ouvrir ce lien sur le téléphone. Android/Chrome : menu ⋮ → Installer l’application ou Ajouter à l’écran d’accueil. iPhone/Safari : Partager → Sur l’écran d’accueil.

## Mettre à jour
Modifier les fichiers dans le même dépôt, puis attendre la fin du déploiement GitHub Pages. Fermer et rouvrir l’application avec Internet : elle demande les fichiers récents avant de consulter sa copie hors ligne. Une partie déjà ouverte garde son code jusqu’à la prochaine ouverture. Aucun changement d’URL ni réinstallation nécessaire. Après une première ouverture en ligne, elle peut fonctionner hors ligne avec la dernière version téléchargée. Lors d’un changement de la liste des fichiers du cache, incrémenter CACHE dans sw.js.

## Jeu v2
- Tables 6 à 10 par défaut, rappel de 2 à 5, sélection personnalisée.
- Cinq résultats uniques, dont exactement un correct. L’opération est en bas ; les bulles descendent en défi, restent fixes en entraînement.
- Une seule tentative : +1 point si juste, −1 si faux ou si les bulles arrivent en bas. Le score peut être négatif.
- Enchaînement automatique : 0,65 seconde après une bonne réponse ; 1,65 seconde après une erreur, avec la correction et la bonne bulle mise en évidence.
- Entraînement de 10 calculs sans chrono. Défi de 120 secondes de jeu actif, avec vitesse 18 / 12 / 8 secondes par calcul. Corrections et pauses suspendent le chrono.
- Interface de jeu dimensionnée à la hauteur disponible du téléphone, sans défilement. L’accueil peut défiler.
- Calculs ratés plus fréquents ; trois réponses justes consécutives indiquent un calcul solide.
- Progression conservée depuis la v1. Points et record remis à zéro au premier lancement v2 car le barème a changé.
- Sauvegarde locale, pas de synchronisation entre appareils.

## Remplacer la v1
Dans le même dépôt GitHub, Add file → Upload files : envoyer les fichiers de cette archive à la racine et Commit changes. Attendre le déploiement Pages, puis fermer et rouvrir le jeu avec Internet. Le numéro v2.0 sur l’accueil confirme la mise à jour. Le raccourci et l’URL restent identiques.
