## [Projet Node.js] Créer une API

Suivi du tuto From Scratch - https://www.youtube.com/watch?v=hjR52rCqlQU

## Init (branche main)

On part d'un dossier vide.

- avant tout : .gitignore avec /node_modules et .env
- npm init -y : création package.json. (-y permet de répondre yes à toutes les questions)
- Création fichier index.js
- npm i -s express nodemon : installation express et nodemon (paquet qui permet de mettre à jour le serveur à chaque enregistremenet). A ce moment-là : création node_modules et package-lock.json
- dans package.json : écriture du script : "start": "nodemon index.js" : à chaque npm start il lancera nodemon : pour vérifier lancer npm start

## Index.js (branche dev)
