# Brainrot Casino — mise en ligne

Le site est gratuit à héberger sur Netlify. Il te faut deux comptes gratuits : GitHub et Netlify.

## 1. Mettre les fichiers sur GitHub
1. Crée un compte sur https://github.com (gratuit).
2. En haut à droite, clique sur **+** puis **New repository**.
3. Nom : `brainrot-casino`. Laisse-le en **Private** si tu veux. Clique **Create repository**.
4. Sur la page du dépôt, clique sur le lien **uploading an existing file**.
5. Dézippe `brainrot-casino-site.zip` sur ton PC, ouvre le dossier, sélectionne **tout ce qu'il y a dedans** (`public`, `netlify`, `package.json`, `netlify.toml`, `LISEZMOI.md`) et glisse-le dans la page GitHub.
6. Clique **Commit changes**.

Vérifie que le fichier `netlify/functions/api.mjs` apparaît bien dans le dépôt.

## 2. Héberger sur Netlify
1. Crée un compte sur https://www.netlify.com avec **Sign up with GitHub**.
2. Clique **Add new project** (ou **Add new site**) puis **Import an existing project**.
3. Choisis **GitHub**, autorise Netlify, puis sélectionne `brainrot-casino`.
4. Ne change aucun réglage (tout est déjà dans `netlify.toml`) et clique **Deploy**.
5. Attends 1 à 2 minutes que le déploiement soit vert (**Published**).

## 3. Mettre le nom « brainrotcasino »
1. Dans ton projet Netlify : **Project configuration** (ou **Site configuration**) → **Change project name**.
2. Tape `brainrotcasino` (ou `brainrot-casino` si c'est pris).
3. Ton site est maintenant sur **https://brainrotcasino.netlify.app**.

## 4. Premier lancement
1. Ouvre le site et connecte-toi tout de suite en **Layola**, mot de passe `123`, puis change le mot de passe.
2. Fais pareil pour **Boruteo** (ou donne-lui l'accès pour qu'il le fasse vite).
3. Les owners ont le **Panel admin** dans le lobby.

## Modifier le site plus tard
- Prix, chances des spins, bonus, coins de départ : en haut du fichier `netlify/functions/api.mjs`.
- Textes et apparence : `public/index.html`.
- Pour mettre à jour : sur GitHub, ouvre le fichier, clique sur le crayon, modifie, **Commit changes**. Netlify remet le site à jour tout seul en 1 minute.

## Bon à savoir
- Les mots de passe sont chiffrés, et les coins, les spins et les droits admin sont gérés par le serveur : un joueur ne peut pas tricher depuis son navigateur.
- Le bannissement bloque le compte **et** les dernières connexions (IP) utilisées par ce compte. Attention : si deux personnes jouent sur le même Wi-Fi, bannir l'une peut empêcher l'autre de créer un compte.
- L'offre gratuite de Netlify suffit largement pour un groupe d'amis.
