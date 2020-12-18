# Dashboard-Covid-17-12-2020

Voici mon projet pour le cours de BI. 
Il s'agit d'un dashboard présentant quelques chiffres sur le Covid-19 lors de ce dernier mois ( dates : 17/11/2020 au 17/12/2020 ).

**Lien** : https://datastudio.google.com/reporting/e3d4e5c7-4acc-4e73-8eab-eb98a54c220b

Il est composé de deux pages : 

* **Global** : Page sur laquelle on retrouvera les informations globales, du monde, liées au Covid ( nombre de décès, chiffres mondiaux, Map monde, évolution des chiffres lors du dernier mois ... ). Il y a un filtre pour comparer les données sur certains pays en particulier (initalisé au monde entier ).

* **Compartif** : Page sur laquelle on pourra comparer les pays entre eux avec des graphiques Bar (nombre max de pays à comparer fixé à 20). Le filtre permet de sélectionner les pays qu'on veut comparer entre eux ( initalisé à 8 : États-Unis Inde France Russie Allemagne Belgique Chine Japon ).

La certification de cours de Google Data Studio a été mise dans le repository.

## Source de données

J'ai choisis une base de données sur le Covid-19, un sujet d'actualité et accessible. 

La source de données est un .csv récupérable à cette adresse : https://coronavirus.politologue.com/data/coronavirus/coronacsv.aspx?format=csv&t=pays ( ou en version finale dans le repository).
Elle donne le nombre d'infections, de décès, de guérisons, ainsi que leur taux dans le monde pour les 30 derniers jours.

J'ai d'abord retravaillé la BDD pour y rajouter 3 colonnes : TotalInfectionsParPays	| TotalDecesParPays |	TotalGuerisonsParPays. 
Je ne pouvais pas choisir la dernière valeur en date sur Google Data Studio alors j'ai choisi de rajouter de la redondance pour me permettre d'avoir la valeur maximale de chaque pays sur chaque ligne.

J'ai importé le fichier .csv avec l'onglet Ressource -> ajouter une source de données -> Importation de fichier.

J'ai ensuite modifié le Type de la dimension Pays en "Pays".
J'ai rajouté 3 champs : Max deces | Moyenne Taux deces | Moyenne Taux de Guerisons 

## Ressources Pédagogiques Externes ou Informatives

* https://www.youtube.com/watch?v=4xmyomDMnnc pour le lancement, l'initialisation du projet. Pour avoir un exemple de création de dashboard.

* https://support.google.com/datastudio/answer/7165560?hl=fr pour avoir des informations sur l'utilisation et la configuration des Graphique à barres.

* https://support.google.com/datastudio/answer/6371135?hl=fr pour gérer et contrôler les accès aux données des utilisateurs.

* https://support.google.com/datastudio/table/6379764?hl=fr pour avoir la liste des fonctions disponibles sur Google Data studio lorsqu'on ajoute un champs dans la source de données.

* https://extremepresentation.com/wp-content/uploads/choosing-a-good-chart-09-1.pdf pour avoir un guide sur le choix des graphiques à utiliser selon les données qu'on veut afficher.

* https://www.youtube.com/watch?v=y1usHXRoD50 pour comprendre comment utiliser un graphique géographique.

* https://coolors.co/e63946-f1faee-a8dadc-457b9d-1d3557 pour avoir des couleurs complémentaires.

* https://www.google.com/search?client=firefox-b-d&q=nombre+de+mort+covid pour comparer ma base de données avec les chiffres actuels. 






