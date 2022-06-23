## [Projet Node.js] Créer une API (Attention MongoDB, pas mySQL)

Suivi du tuto From Scratch - https://www.youtube.com/watch?v=hjR52rCqlQU

## Init

On part d'un dossier vide.

- avant tout : .gitignore avec /node_modules et .env
- npm init -y : création package.json. (-y permet de répondre yes à toutes les questions)
- Création fichier index.js
- npm i -s express nodemon : installation express et nodemon (nodemon paquet qui permet de mettre à jour le serveur à chaque enregistremenet). A ce moment-là : création node_modules et package-lock.json
- dans package.json : écriture du script : "start": "nodemon index.js" : à chaque npm start il lancera nodemon : pour vérifier lancer npm start

## Init de index.js

- Ligne 1 et 2 : on appelle express, et on l'appelera avec constante app par commodité.
- app.listen(5500) : sur le port 5500. Test : le serveur étant démarré (npm start), dans Insomnia voir le GET sur localhost:5500 : il retourne cannot Get... On rajoute un callback à app.listen : console.log pour qu'il nous enforme tourner : on voit ce console.log dans le terminal.

## Init BDD

- Dans mySQL : CREATE DATABASE node_api_from_scratch;
  USE node_api_from_scratch;
  CREATE TABLE `posts` (`id` INT PRIMARY KEY NOT NULL AUTO_INCREMENT, `author` VARCHAR(100) NOT
  NULL, `message` TEXT NOT NULL );
- Retour à VSCode : on va créer connexion à la BDD. Création dossier models et models/dbConfig.js
  (j'arrête là, la suite est en MongoDB)
