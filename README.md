# Groupe-5-NoSQL-B3



Dans ce repo se trouve un Notebook où l'on peut voir les manipulations et agrégations effectuées via Python et PyMongo.

En second, nous pouvons retrouver les fichiers Flask permettant de déployer l'API pour rendre les données accessibles.

Ci-dessous, voici comment utiliser cette API :

--> Route "/" : Permet d'accéder à un formulaire d'insertion de document, on y retrouve également tous les documents listés avec certaines de leurs informations et un bouton pour les supprimer.

--> Route "/search/$variable/$value/" : En précisant l'une des variables (year, last_name, first_name, status, position_title, salary, pay_basis, gender), et une valeur associée à cette variable, nous pouvons effectuer une recherche qui retournera le ou les résultats sous format JSON.
  
--> Route "/findmin/$n/" : Retourne les n résultats ayants les salaires les plus bas, il faut indiquer un entier positif en tant que n.
  
--> Route "findmax/$n/" : Retourne les n résultats ayants les salaires les plus hauts, il faut indiquer un entier positif en tant que n.
  
--> Route "/replace_by_id/$idx/$last_name/$first_name/$year/$status/$pay_basis/$position_title/$salary/$gender/" : Permet de remplacer un document portant l'ObjectID précisé en idx (premier élément à renseigner), puis de fournir les valeurs des champs suivants, dans l'ordre indiqué.
  
--> Route "/replace/$variable/$valeur/$last_name/$first_name/$year/$status/$pay_basis/$position_title/$salary/$gender/" : Permet de remplacer un document ayant la valeur renseignée de la variable renseignée, il faut ensuite fournir toutes les valeurs des champs qui suivent, en respectant l'ordre indiqué.
  
--> Route "/update/$idx/$variable/$valeur/" : Update le champ indiqué en variable avec la valeur indiquée, pour le document portant l'ObjectID renseigné en idx.

--> Route "/$id/delete/" : Supprime le document portant l'id renseigné.
  
  
## Enfin, vous trouverez ci-contre le lien vers le trello où nous nous sommes "répartis" les tâches : https://trello.com/b/Da5hSRO5/nosql-b3-ynov
