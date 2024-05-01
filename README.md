# rest_mediatekdocuments
Cette API est utilisée par l'application MediatekDocuments écrite en C# et récupérable dans le dépôt suivant :
https://github.com/Codeuraxe/MediatekDocuments

## Présentation
[Page de presentation du projet](https://www.bilel-dev.online)

Cette API, écrite en PHP, permet d'exécuter des requêtes SQL sur la BDD Mediatek86 avec MySQL.
Elle utilise une authentification "basique" (login="admin", pwd="adminpwd") et répond aux demandes de l'application MediatekDocuments.

Le projet est un fork de [rest_mediatekdocuments](https://github.com/CNED-SLAM/rest_mediatekdocuments), enrichi de nouvelles fonctionnalités.

## Fichiers de l'API
- **.htaccess** : règles de réécriture pour l'accès à mediatekdocuments.php.
- **Mediatekdocuments.php** : point d'entrée de l'API, gère l'accès sécurisé et les requêtes.
- **Controle.php** : redirige les requêtes aux méthodes appropriées de la classe AccesBDD et renvoie les résultats en JSON.
- **AccesBDD.php** : construit les requêtes SQL, les exécute via ConnexionPDO et renvoie les résultats.
- **ConnexionPDO.php** : gère la connexion à la BDD, prépare et exécute les requêtes SQL.

## Installation de l'API en local
Pour tester MediatekDocuments localement :
- Installer WampServer, Netbeans, Postman.
- Télécharger et dézipper le code de l'API dans le dossier www de WampServer (renommer en "rest_mediatekdocuments").
- Télécharger le script Mission4.sql, créer la BDD mediatek86 via phpMyAdmin et exécuter le script pour configurer la BDD.

