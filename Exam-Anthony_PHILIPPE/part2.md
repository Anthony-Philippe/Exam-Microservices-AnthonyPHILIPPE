Part 2: Microservices Architecture

• Q1: Define what is a Microservices architecture and how does it differ from a Monolithic application.

Une architecture de microservices est une 

Une architecture de microservices est un service logiciel qui structure une application informatique en ensemble de services indépendants (microservices). Ces services gèrent chacun une fonction spécifique de l'application.
Alors qu'une application monolithic regroupe toutes les fonctionnalitées en un seul programme.

• Q2: Compare Microservices and Monolithic architectures by listing their respective pros and cons.

Microservices
Avantages: Modularité, langage de programmation et techniques différentes, indépendance, déploiement et développement rapide, simplicité pour une équipe de développement (chaque développeur peut se concentrer sur un seul service)
Inconvéniens: Complexité pour gérer de nombreux services, latence réseau et utilisation élevée de mémoire, tests plus complexes

Monolithic
Avantages: Simplicité de construction, tests plus simple, enregistrement de logs, bonnes performances et partege de mémoire donc plus rapide en communication
Inconvéniens: Faible fiabilité car si une erreur dans un module cela peut rendre l'application inutilisable, mise à jour compliqué avec les dépendance entres les composants, utilisation d'un seul langage / technologie ce qui rend complexe sa modification en cas de besoin


• Q3: In a Micoservices architecture, explain how should the application be split and why.

L'application doit être divisée en services indépendants (microservice) qui ont une fonctionnalités spécifiques et langage et des technologies propres.
Chaque microservice peut être développé, déployé indépendamment des autres qui facilite la maintenance car cela n'affecte pas les autres services.
Les microservices avec des fonctionnalités similaire peuvent être regrouper et permet de réduire la duplication de code et avoir une meilleure efficacité.

• Q4: Briefly explain the CAP theorem and its relevance to distributed systems and Microservices.

Le théoreme CAP (Consistency, Aailability, Partition Tolerance) est un concept en informatique qui dit qu'il est impossible sur un système de calcul de garantir en même temps les contraintes de cohérence, de disponibilité et de tolérance aux partitions.
Cohérence: tout les services d'un système recoivent les même données au même moment.
Disponibilité: tout le système répond toujours aux requêtes même en cas d'erreur.
Tolérance de partionnement: tout le système doit continuer de fonctionner même si certaines parties du réseau ne peuvent plus communiquer.
Il est pertinent pour les systèmes distribués et microservices car ils ont souvent des problèmes de cohérence ou de disponibilité, comme les microservices communiquent en réseau ils sont susceptible d'avoir des problèmes.

• Q5: What consequences on the architecture ?
L'architectures de microservices doit faire des compromis en termes de cohérence et de disponibilité. C'est à dire qu'il faut faire un choix sur la manière de gérer les mises à jour de données et la synchronisation entre les services mais cela peut avoir un impact sur les performences.


• Q6: Provide an example of how microservices can enhance scalability in a cloud environment.

Ils peuvent améliorer la scalabilité d'un environnement cloud car chaque service sont indépendamment mis à l'échelle. C'est à dire si un service a une augmentation de requète il peut être mis à l'échelle en ajoutant des instances à lui uniquement sans affecter d'autre services

• Q7: What is statelessness and why is it important in microservices architecture ?

Le statelessness est le fait qu'un microservice ne conservce pas d'informations sur l'application car chaque requête sont traitées de manière indépendante.
C'est important car cela permet une meilleur scalabilité, ils peuvent être facilement mis à l''échelle et avoir une simplicité de gestion d'erreurs.

• Q8: What purposes does an API Gateway serve ?

Une API Gateway permet d'agréger les services en un interface pour pouvoir intérargir avec tous en même temps, la communication et complexité d'utilisation est réduit.
Il y a également une meilleure securité car elle peut gérer l'authentification et les autorisations pour les utilisateurs d'accès à un service. Et également les protections contre les attaques DDos ou injections de code.
Et enfin cela permet la gestion du trafic en répartissant la charge du trafic entre les services en fonction de leur capacités (meilleur performances). Mais aussi la transmission de données (conversion, agrégé, communication etc...)