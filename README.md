# Projet JEE et Systèmes Distribués

![key](https://user-images.githubusercontent.com/33198285/215280003-f884c452-a3af-452e-ba12-5a5134dd42fb.PNG)


Introduction
------------

Ce projet est une architecture de microservices utilisant Spring Cloud et Angular. Le projet consiste à créer plusieurs microservices et une passerelle pour les gérer, ainsi qu'un service de découverte et un service de facturation en utilisant Open Feign. Le projet comprend également le déploiement de Keycloak pour la sécurité et la création d'un client web en utilisant Angular.

Microservices
-------------

1.  customer-service: Ce microservice est responsable de la gestion des clients. Il inclut des opérations CRUD pour les clients et leurs informations.
2.  inventory-service: Ce microservice est responsable de la gestion des produits. Il inclut des opérations CRUD pour les produits et leurs informations.

Gateway
-------

1.  Spring Cloud Gateway: C'est la passerelle principale pour les microservices. Il inclut une configuration de routage statique pour les microservices.
2.  Eureka Discovery Service: Ce service est utilisé pour la découverte et l'enregistrement des services. Il permet aux microservices de se trouver et communiquer facilement entre eux.

Configuration de routage
------------------------

1.  La configuration de routage dynamique est mise en œuvre en utilisant Spring Cloud Gateway. Il permet de mettre à jour et gérer facilement le routage des microservices.

Service de facturation
----------------------

1.  Billing-Service: Ce service est responsable de la gestion des factures et des paiements. Il utilise Open Feign pour communiquer avec d'autres microservices.

Client web
----------

1.  Client web Angular: C'est un client web pour les microservices. Il inclut une interface utilisateur pour les clients, les produits et les factures.

Sécurité
--------

![sign in key](https://user-images.githubusercontent.com/33198285/215280027-76c7e52b-daf7-43c5-a2cc-ae94dfbd4dac.PNG)

1.  Keycloak: C'est une solution open-source d'identité et d'accès. Il est utilisé pour sécuriser les microservices et le client web Angular. Les étapes suivantes sont effectuées pour sécuriser le système:

-   Créer un Realm
-   Créer un client à sécuriser
-   Créer des utilisateurs
-   Créer des rôles
-   Assigner des rôles aux utilisateurs
-   Tester différents modes d'authentification en utilisant Postman et montrer le contenu de Access-Token et Refresh Token

KAFKA
-----

![kafka](https://user-images.githubusercontent.com/33198285/215280037-4e94df89-5850-4420-a795-71b39a32a554.PNG)

Mettre en place une architecture de traitement de données en temps réel à l'aide de KAFKA.

Installation et configuration de KAFKA
--------------------------------------

-   Télécharger et installer la distribution officielle de KAFKA sur votre système.
-   Configurer les paramètres de votre cluster KAFKA.

Développement d'un Micro-service "Billing-Service"
--------------------------------------------------

-   Développer un micro-service qui publie les factures dans un Topic KAFKA.
-   Consommer les factures publiées dans le Topic KAFKA et les enregistrer dans sa propre base de données.

Développement d'un Micro-service "Data-Analytics-Service"
---------------------------------------------------------

-   Utiliser l'API KAFKA Streams pour effectuer du traitement en temps réel des flux de données de factures publiées dans le Topic KAFKA.

Utilisation
-----------

Pour utiliser ce projet, vous devez d'abord suivre les étapes d'installation et de configuration de KAFKA. Ensuite, vous pouvez développer les micro-services "Billing-Service" et "Data-Analytics-Service" et utiliser l'interface frontale pour visualiser les résultats obtenus.

Note
----

Il est important de noter que ce projet nécessite une certaine connaissance de KAFKA et de ses fonctionnalités pour être correctement mis en place et utilisé. Il est recommandé de consulter la documentation officielle de KAFKA avant de commencer ce projet.

Déploiement
-----------

Tous les services et la passerelle peuvent être déployés en utilisant un outil de déploiement tel que Docker ou Kubernetes pour une exécution en production. 

Conclusion
----------

En résumé, ce projet est un système de microservices basé sur Spring Cloud et Angular, avec un service de découverte Eureka, un service de facturation Open Feign, une passerelle Spring Cloud Gateway et une sécurité intégrée grâce à Keycloak.
Il permet de créer et gérer des clients et des produits, ainsi que de gérer les factures. Il est important de configurer et tester correctement tous les services avant le déploiement.

Ce projet a été créé par **Zohair Diab**, avec l'aide de **ChatGPT** **&copy;**
