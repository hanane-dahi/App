# Le temps réel sur le web : NodeJS
L’application à développer doit permettre à ses utilisateurs d’interagir avec le serveur pour lui demander
d’exécuter des requêtes sur son système de fichiers et retourner les résultats en les affichant sur la fenêtre
du navigateur client. Pour pouvoir utiliser l’application, un utilisateur doit d’abord s’inscrire auprès du
système en introduisant son nom et son prénom et en choisissant un login et un mot de passe pour des
fins d’authentification. Les informations saisies par l’utilisateur doivent être inscrites dans une collection en
mémoire ou dans une base de données NoSQL telle que MongoDB.
Les utilisateurs possédant un compte dans le système peuvent accéder à un ensemble de
fonctionnalités/services en fournissant l’URI correspondant (login, logout, upload, show, find, …). Le
service login doit servir à ouvrir une session avec le serveur alors le service logout permet de mettre fin à la
session courante. Le service upload permet à l’utilisateur de choisir une image pour son profil et la
sauvegarder sur le disque du serveur pour pouvoir la retourner plus tard. Le service show, quant à lui,
permet à l’utilisateur de retourner et afficher sur son navigateur la dernière image qu’il a chargée sur le
serveur, sinon une image par défaut sur le système de fichiers. Enfin, le service find doit être demandé par
l’utilisateur lorsqu’il veut afficher sur son navigateur l’ensemble des fichiers du serveur. Il est à noter que si
l’utilisateur ne spécifie pas le service demandé lors de la formulation d’une requête (c’est-à-dire, seul l’URL
du serveur est indiqué) le serveur lui affichera un message d’accueil avec possiblement l’ensemble des
services disponibles. Par contre, lorsque l’utilisateur demande un service non-existant le serveur lui
présentera un message d’erreur.