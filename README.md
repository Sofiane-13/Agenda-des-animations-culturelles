# Agenda-des-animations-culturelles

# Introduction
Le projet a pour but de mettre en place un entrepôt de données à partir d’un fichier CSV ou JSON récupéré sur un opendata, après quelques heures de recherche en ligne nous avons opté pour les données suivants : “Agenda des animations culturelles de la Bibliothèque Municipale de la ville de Nantes”.

lien : http://data.nantes.fr/donnees/detail/agenda-des-animations-culturelles-de-la-bibliotheque-municipale-de-la-ville-de-nantes/

Nous mettrons en pratique tous les concepte liés à la BI appris dans ce module, pour cela nous utiliserons les outils tels que :
ORACLE.
SQLDEVELPPEUR.

# présentation de projet 
Nantes aujourd’hui est l’une des plus grandes villes culturelles de France, on y retrouve pleins de spectacle de tous genres dans l’agenda des animations culturelles de la Bibliothèque Municipale de Nantes, pour améliorer la qualité d’année en année du programme les élus ont besoin de remonter un certain nombre d’informations pertinentes facilement et rapidement  et c’est là qu’on intervient avec notre solution.

# Description des démarches à suivre pour arriver à un entrepôt de données
L’objectif de ce projet est :
la conception du schéma de notre entrepôt de données après une étude des informations que l’on dispose.
l’extraction, la transformation et le chargement des données sur notre entrepôt de données.
l’exploitation de ces données ( écrire des requêtes pertinente ).

# Conception du schéma de l'entrepôt
Nous disposons du fichier CSV qui contient tous les informations de l’agenda des animations culturelles, à partir de ces données-là nous avons pu construire notre table de fait et nos tables de dimension.
Shéma : https://github.com/Sofiane-13/Agenda-des-animations-culturelles/blob/master/monshema.jpg

# Processus

# Etape 1 : 

Importation du fichier CSV dans la base de donnée ( table agenda )

# Etape 2 :

À partir de notre table agenda on fait des insertions dans les tables dimensions et la table de fait, pour certaines insertions on utilise le PL/SQL afin de verifier, si le format des attributs est adéquat on fait l'insertion, sinon on insere la ligne dans une table rejet.

# Pré-requis

Avoir Oracle SQL Developer sur sa machine.

# Installation

Executer export.sql dans l'outil Oracle SQL Developer

# Tester

Les requets se trouvent dans le fichier requetes.txt

Le nombre d'événements par tranche : https://github.com/Sofiane-13/Agenda-des-animations-culturelles/blob/master/evenementpartranche.png
