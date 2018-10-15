# Affichage, ajout et modification de données 

## Présentation

La section "Data" permet l'ajout et la modification de données du catalogue. Pour y accéder, 
cliquer sur "*Data*" dans la barre de menus noire (en haut du navigateur). 

L'accueil de la section **Data** consiste en un affichage des différentes fiches existantes dans la barre latérale gauche. 

## Affichage des tableaux de données

Dans la section *Data* la barre latérale gauche permet d'accéder aux données par fiches. Une fois la fiche choisie, une liste des données existantes est présentée. 

![](assets/captures_CATIMA/data/data.PNG)

> NB : Certains champs ont pu être cachés dans la configuration du type de fiche. Ainsi seuls Les champs pour lesquels l'option "Inclure le champ dans la liste des fiches" a été activée dans ***Setup*** seront affichés dans cette liste.

## Ajout de données

Pour ajouter des données, sélectionner le type de fiche souhaité dans la barre latérale gauche. Les éventuelles données existantes s'affichent sous forme de tableau. Dans le cas contraire, une section vide apparaît en dessous du nom de la fiche.

Une fois la fiche sélectionnée, cliquer sur le bouton  **Nouveau type de fiche "nom du type de fiche"**, fait s'ouvrir la page d'entrée manuelle des données, qui se présente sous la forme d'un formulaire.

En remplissant les sections des objets avec des données, seules des données respectants les formats autorisés (définis dans la configuration) peuvent être entrées (p.ex données numériques, e-mail ou dates).

Une fois les champs remplis avec les données, il est possible d'enregistrer et retourner au menu *Data* avec "*Créer fiche de type 'nom du type de fiche'*" ou d'enregistrer et ajouter de nouvelles données avec "*Create and add another*".

> NB : Il est possible d'annuler à tout moment en cliquant sur "Annuler" (Cancel).

![](assets/captures_CATIMA/data/new_data_1.PNG)  
![](assets/captures_CATIMA/data/new_data_2.PNG)  


Une fois les champs remplis, enregistrer avec " *Enregistrer 'nom du type de fiche'* ". Un enregistrement n'est possible que si toutes les sections obligatoires ont été remplies. Dans le cas contraire un message d'erreur apparaît et invite à corriger ou remplir les champs.

Une fois les données enregistrées, celles-ci apparaissent dans la section *Data* sous la forme d'un tableau de données. 

## Modification de données

Pour choisir les données à modifier, sélectionner la fiche souhaitée dans la barre latérale gauche. Les données existantes s'affichent sous forme d'un tableau. Pour modifier la fiche souhaitée, cliquer sur le bouton "Actions" puis sur "Éditer" :

![](assets/captures_CATIMA/data/edit_data.PNG)  

Pour la modification de chaque champ, la procédure et les remarques sont semblables à l'ajout de données (voir [Ajout de données](#ajout-de-données)).

Une fois les modifications terminées, enregistrer avec " *Enregistrer 'nom du type de fiche'* ". Un enregistrement n'est possible que si toutes les sections obligatoires ont été remplies. Dans le cas contraire un message d'erreur apparaît et invite à corriger ou remplir les champs.

Une fois les données enregistrées, celles-ci apparaissent dans la section *Data* sous la forme d'un tableau de données. 

## Duplication de données

Il est possible de dupliquer une fiche en cliquant sur le bouton "Actions" puis sur "Dupliquer" : 

![](assets/captures_CATIMA/data/duplicate_data.PNG)  

Cela ouvre la même page que pour l'ajout de données, avec les données de la fiche dupliquée, qu'il est possible de modifier.

Une fois les champs modifiés, il est possible d'enregistrer et retourner au menu *Data* avec "*Créer fiche de type 'nom du type de fiche'*" ou d'enregistrer et ajouter de nouvelles données avec "*Create and add another*".

# Exemple d'ajout de données dans un catalogue

Afin d'illustrer l'ajout de données dans un catalogue, voici un exemple reprenant toutes les étapes décrites jusqu'à présent. Cet exemple consiste en un catalogue recensant les universités romandes et de leurs bibliothèques afin de les représenter sur une carte géographique.

## Concept

Les informations que le catalogue devra contenir à la fin sont les suivantes : 

|  | Université de Fribourg | Université de Genève | Université de Lausanne | Université de Neuchâtel |
|--------------------|--------------------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Abbréviation | UNIFR | UNIGE | UNIL | UNINE |
| Localité | Fribourg | Genève | Lausanne | Neuchâtel |
| Bâtiments | Uni Beauregard, Uni Miséricorde, Uni Pérolles, Uni Régina Mundi |Battelle, Campus Biotech, CMU, Les Philosophes, Sciences, Uni Bastion, Uni Carl Vogt, Uni Dufour, Uni Mail, Uni Pignon |Amphimax, Amphipôle, Anthropole, Batochime, Biophore, Cubotron, Génopode, Internef, Unicentre, Unithèque|Rue de Saint-Nicolas 4, Place Numa-Droz 3, Chaussée de la Boine 20 , Fbg du Lac 5a, Av. DuPeyrou 1, etc.. |
| Facultés |Droit, Lettres et sciences humaines, Sciences et médecine, Sciences économiques et sociales, Théologie |Droit, Économie et management, Lettres, Médecine, Psychologie et sciences de l'éducation, Sciences, Sciences de la société, Théologie |Biologie et médecine, Droit, sciences criminelles et administration publique, Géosciences et environnement, Hautes études commerciales, Lettres, Sciences sociales et politiques, Théologie et sciences des religions  |Droit, Lettres et sciences humaines, Sciences,Sciences économiques |
| Nombre d'étudiants | 10414 |  16935 | 14976 | 4284 |
| Bibliothèque | Bibliothèque cantonale et universitaire (Fribourg) | Bibliothèque de l'Université de Genève | Bibliothèque cantonale et universitaire (Lausanne) | Bibliothèques UniNE |
| Adresse | Avenue de l'Europe 20, 1700 Fribourg | 24 rue du Général-Dufour,   1211 Genève 4 | Unicentre, 1015 Lausanne | Avenue du 1er-Mars 26, 2000 Neuchâtel |
| Site web | www.unifr.ch | www.unige.ch | www.unil.ch | www.unine.ch |

Dans cet exemple, les concepts d'Université et de Bibliothèque sont centraux dans ce catalogue. 

Conceptuellement, voici les entités qui composent ce catalogue et les champs qu'il s'agira de remplir.

|Localité
|---
|Nom de la localité
|Canton
|Population
---

|Université
|---
|Nom de l'Université
|Abbréviation
|Localité ==> **concept "Localité"**
|Facultés
|Nombre d'étudiants
|Photographies
|Adresse
|Site web
----

|Bâtiment
|---
|Nom du bâtiment
|Localisation géographique
|Université ==> **concept "Université"**
---

|Bibliothèque
|---
|Nom de la bibliothèque
|Abbréviation
|Réseau
|Bâtiment ==> **concept "Bâtiment"**
|Université  ==> **concept "Université"**
---

### Types de fiches et liens

Les quatre concepts précédements relevés, "Université", "Bibliothèque", "Localité", "Bâtiment", correspondent aux types de fiches existants dans Catima.

**Liens conceptuels entre les types de fiches :**

* Une **localité** a une et une seule **université**
* Une **université** a une, ou plusieurs **bibliothèque(s)**
* Une **université** a un, ou plusieurs **bâtiment(s)**

### Ajout d'une fiche

Le concept de "Localité" étant le concept le plus large (un bâtiment se situe dans une université, qui est dans une localité), il englobe les concepts plus précis que lui, à savoir "Université", qui lui-même englobe les "Bâtiments" et les "Bibliothèques". C'est pourquoi il est judicieux d'ajouter d'abord des fiches aux entités les plus larges, ici "Localité". Ainsi lors de l'ajout d'une nouvelle université (puis de nouveaux bâtiments et bibliothèques) il existera toujours l'entité plus globale à laquelle faire référence. 

La structure du catalogue a été crée dans cet exemple par l'adminstrateur-trice du catalogue. La tâche ici est d'ajouter de nouvelles données en suivant la structure existante. 

Ainsi pour ajouter une nouvelle localité : dans la section "Data" de Catima, sélectionner "Localités" dans la colonne latérale gauche. 

Une liste des localités existante s'affiche : 

![](assets/captures_CATIMA/data/new_data_ex1.PNG)  

Cliquer sur "+ Nouveau type de fiche 'Localité'" puis remplir tous les champs nécessaires : 

![](assets/captures_CATIMA/data/new_data_ex2.PNG)  

Une fois la localité créée, il est possible de lui ajouter l'Université dans la localité de Lausanne :

![](assets/captures_CATIMA/data/new_data_ex3.PNG)  

Puis d'ajouter les données des autres types de fiches "Bâtiments" et "Bibliothèques" : 

![](assets/captures_CATIMA/data/new_data_ex4.PNG)  

