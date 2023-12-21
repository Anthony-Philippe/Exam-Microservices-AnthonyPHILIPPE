J'ai un problème avec docker sur mon ordinateur, j'ai perdu ma clé d'authentification et impossible de mettre la main dessus donc je vous met les commandes que j'ai utilisé pour la partie de création d'une image docker dans ce fichier et tout le dossier sur github en accès publique.
Merci de votre compréhension.

commande effectuer pour la partie 1 - docker:

docker build -t examanthonyphilippe:V1.0 .
docker run -p 8081:8081 examanthonyphilippe:V1.0 