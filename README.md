# Labyrinthe

Le code se divise en deux parties :

Pour commencer, la première partie établit une connexion à un serveur à l'aide d'un socket client. Le message de souscription est envoyé au serveur via le socket client et une réponse est renvoyée par le serveur. Si la réponse contient une erreur, le message d'erreur est affiché. Ensuite, un délai d'une seconde est introduit, suivi de l'impression du message "pong".

Ensuite, la deuxième partie du code utilise un socket serveur qui est utilisé pour écouter les connexions entrantes sur un port spécifié. Si une connexion est établie, le serveur reçoit un message du client, qui est analysé à l'aide du module json. Si le message contient une demande de "ping", le serveur envoie une réponse "pong" au client. La boucle continue à écouter les connexions entrantes jusqu'à ce qu'une exception de temps d'attente soit levée.# Labyrinthe
