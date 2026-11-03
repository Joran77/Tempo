# Tempo : installation sur GitHub Pages

Tempo est une application web installable : une fois en ligne, chacun l'ouvre depuis son navigateur et l'ajoute à son écran d'accueil comme une vraie application. Les données de chaque personne restent sur son propre téléphone.

## 1. Créer le dépôt (une seule fois)

1. Crée un compte gratuit sur https://github.com si tu n'en as pas.
2. En haut à droite, clique sur **+** puis **New repository**.
3. Nom du dépôt : `tempo`. Coche **Public** (obligatoire pour GitHub Pages gratuit). Laisse le reste par défaut et clique sur **Create repository**.

## 2. Envoyer les fichiers

1. Dans le dépôt vide, clique sur le lien **uploading an existing file**.
2. Décompresse l'archive `tempo-github.zip` sur ton ordinateur, ouvre le dossier `tempo` obtenu, puis sélectionne **tout son contenu** (`index.html`, `manifest.webmanifest`, `sw.js`, `README.md`, et les dossiers `icons` et `news`) et fais-le glisser dans la page GitHub. Ne glisse pas le dossier `tempo` lui-même.
3. En bas, clique sur **Commit changes**.

Astuce : le fichier `.nojekyll` est caché sur certains ordinateurs. S'il n'est pas envoyé, ce n'est pas grave.

## 3. Mettre en ligne

1. Dans le dépôt, va dans **Settings**, puis **Pages** (menu de gauche).
2. Sous **Build and deployment**, choisis **Source : Deploy from a branch**, puis **Branch : main** et le dossier **/ (root)**. Clique sur **Save**.
3. Attends une à deux minutes et recharge la page : l'adresse s'affiche en haut, sous la forme `https://ton-pseudo.github.io/tempo/`.

## 4. Installer sur le téléphone

- **Android (Chrome)** : ouvre l'adresse, puis menu **⋮** et **Installer l'application** (ou **Ajouter à l'écran d'accueil**).
- **iPhone (Safari)** : ouvre l'adresse, touche le bouton **Partager**, puis **Sur l'écran d'accueil**.
- **Ordinateur (Chrome ou Edge)** : une icône d'installation apparaît à droite de la barre d'adresse.

Après la première ouverture, Tempo fonctionne aussi sans connexion.

## 5. Récupérer tes données depuis la version Claude

1. Dans Tempo ouvert depuis Claude : bouton de réglages (flèche vers le bas, en haut à droite), puis **Copier les données**.
2. Envoie-toi ce texte (mail, note, message).
3. Dans Tempo installé : même bouton, colle le texte dans **ou coller les données**, puis **Remplacer tout**.

Ton thème est propre à chaque appareil : choisis-le de nouveau avec le bouton palette.

## 6. Partager avec tes amis

Envoie-leur simplement l'adresse `https://ton-pseudo.github.io/tempo/`. Au premier lancement, Tempo leur demande leur prénom et s'ils veulent garder les exemples. Leurs données restent sur leur téléphone : tu ne les vois pas, et ils ne voient pas les tiennes.

## 7. Le point d'actualité

Le dossier `news` contient les points d'actualité (un fichier par jour, plus `index.json` qui en tient la liste). Pour que le point du matin arrive aussi dans cette version, donne à Claude l'adresse de ton dépôt : la tâche de 6 h 39 y ajoutera chaque jour le nouveau fichier.

## 8. Mettre à jour l'application

Quand une nouvelle version est prête, remplace `index.html` (et `sw.js` s'il a changé) avec **Add file**, puis **Upload files**. Les téléphones récupèrent la nouvelle version au lancement suivant.
