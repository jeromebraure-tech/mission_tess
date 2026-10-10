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

## Jeu
- Tables 6 à 10 sélectionnées au départ ; multiplicateurs 1 à 10. Rappel des tables 2 à 5, sélection personnalisée.
- Entraînement : 10 questions sans chrono. Défi : 120 secondes de temps de réponse actif, 18 / 12 / 8 secondes par bulle ; la lecture de la correction et les pauses arrêtent le chrono. La durée réelle peut donc dépasser deux minutes.
- Réponse saisie sur pavé tactile ou clavier ; validation explicite. Correction après chaque tentative et bouton Continuer.
- Les calculs avec erreurs sont davantage tirés au sort. Trois réponses correctes sans indice rendent un calcul « solide » ; une erreur ou une réponse avec indice remet sa série à zéro. Cet indicateur représente la progression dans le jeu, pas une évaluation scolaire.
- Étoiles, objectif quotidien de 10 réponses correctes, record du défi (toutes vitesses et tables confondues). Pas de perte d’étoiles.
- Sauvegarde locale uniquement : pas de compte ni transfert entre appareils. Effacer les données du navigateur efface la progression. Le jeu fonctionne aussi sans sauvegarde si celle-ci est bloquée.
- Mise en pause quand on change d’onglet. Pas de publicité, suivi, sons ni données envoyées à un serveur applicatif.

## Fichiers
Tout le style et la logique du jeu sont dans index.html. Les fichiers complémentaires servent à l’installation et au fonctionnement hors ligne. Pour essayer sans hébergement, ouvrir index.html : le jeu fonctionne, mais l’installation et le service worker demandent HTTPS (ou localhost).
