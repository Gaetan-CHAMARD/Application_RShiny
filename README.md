# Application_RShiny
Documentation fonctionnelle (orientée utilisateur)

Comment fonctionne l’application ?

Celle-ci comporte 3 onglets 

Le premier (le principal) comporte une carte de la ville de lyon où l’on peut choisir l’arrondissement que l’on souhaite et le paiement par carte bancaire, les stations velo’v s’affiche automatiquement avec des repères permettant de connaître le nombre de velo’v disponible dans cette station.
Sur ce même onglet, on peut retrouver un histogramme qui met en lumière le nombre de velo’v disponible selon les arrondissements, et suivant les stations si nous filtrons à un seul et même arrondissement. Un bouton permettant de rafraîchir les données est présent afin que l’application soit plus réaliste et utilisable à tout moment.

Le deuxième onglet est un tableau de bord, il permet d’afficher des statistiques globales sur le nombre total de station présentes à lyon et le nombre de velo’v disponible dans les stations (la somme générale). On peut aussi retrouver un histogramme qui permet de comparer le nombre de station par commune avec un filtre qui permet de sélectionner les communes que l’on souhaite. Et enfin, si on le souhaite, nous pouvons exporter le graphique en format PNG grâce à un bouton.

Le dernier et troisième onglet permet de prendre connaissance de la base de données brute. On peut la visualiser et comprendre le format des variables/attributs avec un tableau. Et enfin, si on le souhaite, nous pouvons exporter la base de données en format CSV en cliquant sur un bouton.

Documentation Technique (Orientée pour Développeur)
Application Shiny "Vélo'v in Lyon"
Cette documentation technique a pour objectif d'expliquer en détail la structure et le fonctionnement de l'application Shiny "Vélo'v in Lyon" qui permet de visualiser les données relatives aux stations Vélo'v à Lyon. Elle comprend des informations sur les packages utilisés, la connexion à la base de données, la création des tables, les composants de l'interface utilisateur, et la logique du serveur Shiny.
Packages Utilisés
L'application utilise plusieurs packages R pour son fonctionnement. Voici la liste des packages requis, avec une brève description de leur rôle :
•	RMySQL: Package pour la connexion à une base de données MySQL.
•	httr: Utilisé pour effectuer des requêtes HTTP et récupérer des données de l'API JCDecaux.
•	jsonlite: Pour traiter les données JSON récupérées de l'API.
•	readr: Utilisé pour la lecture de données.
•	shiny: Le framework Shiny pour la création de l'interface.
•	leaflet: Package pour la création de cartes interactives.
•	sf: Pour le traitement de données géospatiales.
•	tidygeocoder: Pour le géocodage inverse des coordonnées.
•	tidyverse: Une collection de packages pour la manipulation de données.
•	plotly: Pour créer des graphiques interactifs.
•	shinydashboard: Extension de Shiny pour la création de tableaux de bord.
•	shinyjs: Pour ajouter des fonctionnalités JavaScript à l'application Shiny.
•	DT: Pour la création de tables de données interactives.

Application disponible sur ShinyApps.io :  https://velovlyon.shinyapps.io/test_application/
