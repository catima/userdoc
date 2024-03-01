Afin d'illustrer la réalisation d'un catalogue du début à la fin, voici un exemple reprenant la plupart des étapes décrites jusqu'à présent. Cet exemple consiste en un catalogue recensant les universités romandes et de leurs bibliothèques afin de les représenter sur une carte géographique.

<a id="conceptualisation"></a>
## Conceptualisation 

Une manière de débuter la conceptualisation est de représenter des données réelles ou d'exemple sous la forme d'un tableau de données. Cette étape de création fera émerger les éléments marquants du catalogue.

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

Dans cet exemple, la réalisation d'un tableau permet de relever les concepts importants de ce catalogue. Les concepts d'Université et de Bibliothèque sont centraux dans ce catalogue. Les grandes lignes du catalogue sont ainsi tracées conformément à son but initial ("Créer une base de données des Universités romandes et de leurs bibliothèques afin de les représenter sur une carte géographique"). Mais pour décrire une université, certains autres concepts méritent également d'être décrits comme la localité où se situe l'université ou ses bâtiments.

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

<a id="typesfichesliens">
### Types de fiches et liens

Les quatre concepts précédements relevés, "Université", "Bibliothèque", "Localité", "Bâtiment",  correspondent aux types de fiches qu'il faudra créer dans CATIMA.

**Liens conceptuels entre les types de fiches :**

* Une **localité** a une et une seule **université**
* Une **université** a une, ou plusieurs **bibliothèque(s)**
* Une **université** a un, ou plusieurs **bâtiment(s)**

Cette structure permet d'afficher toutes les bibliothèques, ainsi que tous les bâtiments d'une université.

<a id="typesdeficheschamps"></a>
## Ajout des types de fiches et création de champs

> Pour cette étape, se baser sur la section "Ajout d'un type de fiche". 

> NB : Cet exemple propose un catalogue bilingue français/anglais. Pour un catalogue mono- ou plurilingue, remplir les champs correspondants aux langues du-dit catalogue.

Le concept de "Localité" étant le concept le plus large (un bâtiment se situe dans une université, qui est dans une localité), il englobe les concepts plus précis que lui, à savoir "Université", qui lui-même englobe les "Bâtiments" et les "Bibliothèques". C'est pourquoi il est judicieux de créer d'abord le type de fiches de l'entité la plus large, ici "Localité". Ainsi lors de l'ajout d'une nouvelle université (puis de nouveaux bâtiments et bibliothèques) il existera toujours l'entité plus globale à laquelle faire référence.

Il s'agit ici de donner un nom (et d'éventuelles traductions du nom) au type de fiche, des formes au pluriel, ainsi qu'une version courte du nom appelée "slug" (NB : la langue anglaise se prête souvent bien à cet usage) puis de confirmer avec le bouton "créer type de fiche". 

 ![](assets/setup/new_item_type_ex1.png)

 Le type de fiche "Localité" ainsi créé est par défaut vide : 

  ![](assets/setup/new_item_type_ex2.png)

La prochaine étape est donc d'ajouter des champs descriptifs, qui ont été déterminés dans l'étape de conceptualisation. Pour la "Localité", il s'agira ainsi de créer les champs "Nom de la localité", "Canton" et "Population".

Pour cela, cliquer sur le bouton "+Ajouter", qui affichera une liste de champs possibles à ajouter. Le champ "Nom de la localité" par exemple sera un champ "de texte" et "Population" sera un champ "nombre entier". Pour le champ "Canton", ceux-ci étant en nombre limités (4), un champ "ensemble de choix" semble indiqué, mais un champ de texte aurait très bien convenu également.

Pour le champ "Nom de la localité", remplir le nom du champ (et éventuelles traductions), les formes au pluriel et le slug. Il est également possible d'ajouter un texte d'aide à la saisie, et de spécifier des options d'affichage comme définir que le champ en question comme champ primaire (voir "champ primaire"). Noter également les options de saisie de données, qui permettent selon le type de champ, d'entrer une ou plusieurs données (Single vs Multiple values) et de s'assurer que le champ sera rempli par l'utilisateur (Required). Confirmer l'ajout d'un champ avec le bouton "Créer le champ".

  ![](assets/setup/new_item_type_ex3.png)
  ![](assets/setup/new_item_type_ex4.png)

Cette étape, à répéter pour chaque champ du type de fiche, est globalement similaire pour tous les champs, voir "Types de champs" pour les spécifités de chaque champ.

Une fois tous les champs d'un type de fiche créés, créer un nouveau type de fiche par ordre de complexité croissante, jusqu'à avoir créé tous les types de fiches avec tous leurs champs. 

<a id="referenceautrechamp"></a>
### Références à d'autres champs 

Lors de la conceptualisation, les concepts les plus "précis" comme par exemple "Bâtiment", font référence aux concepts dans lesquels ils sont compris, par exemple ici "Université". On attribue ainsi à chaque bâtiment une caractéristique d'appartenance à une université.

Dans CATIMA cela se traduit par la création d'un champ "Référence" : 

> Dans notre exemple, il s'agira dans "Bâtiment" de faire une référence aux concepts d' "Université". 

Pour cela, sélectionner "Bâtiment" parmi les types de fiches (accessibles dans la barre latérale gauche) puis créer un nouveau champ "Référence". 

  ![](assets/setup/new_item_type_ex5.png)

Pour l'éditeur de données, cela se concrétisera dans l'ajout d'un nouveau bâtiment par la possiblité/obligation de choisir parmi les universités pré-existantes.