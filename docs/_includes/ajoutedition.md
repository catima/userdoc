Un type de fiche peut avoir des caractéristiques communes à toutes les données (p.ex : tous les films ont un réalisateur) mais peut également avoir des caractéristiques "conditionnelles" (p.ex : la 'Période traitée' n'est pertinente que pour les documentaires historiques et pas pour les films d'action). Dans ce dernier cas, il est possible de créer une **sous-fiche** qui s'affiche uniquement lorsqu'un certain **choix** est sélectionné (p.ex : le choix de 'Période traitée' apparaît uniquement si le choix documentaire historique est sélectionné et reste invisible si le choix film d'action est sélectionné).

Cela permet de ne pas avoir de champs superflus lors de la saisie de données. 

Pour permettre l'enregistrement de données de manière conditionnelle, il est nécessaire de:
  1. D'abord créer la **sous-fiche**
  2. Puis créer l'**ensemble de choix** dans la fiche principale.  

> Il n'est pas possible de créer une sous-fiche à partir d'une autre condition qu'un ensemble de choix dans la fiche principale. 

<a id="creationsousfiche"></a>
### 1. Création d'une sous-fiche 

> La notion de sous-fiche étant liée à celle de type de fiche, se référer si besoin à la section "Type de fiche".

Pour ajouter une **Sous-fiche** , dans la barre de gauche, en bas de la rubrique "*Sous-fiches*", cliquer sur "**+ Nouvelle sous-fiche**". 

![](assets/categories/new_category.png)

Une fois choisi un nom pour la sous-fiche, il est possible d'enregistrer et retourner au menu *Setup* avec "*Créer sous-fiche'*" ou d'enregistrer et ajouter une nouvelle sous-fiche avec "*Create and add another*".
 
<a id="editionsousfiche"></a>
### Édition d'une sous-fiche

Une fois la/les sous-fiches créée-s, il s'agit d'y ajouter les champs souhaités. 

![](assets/categories/edit_category.png)

La procédure est similaire à celle de l'édition d'une fiche et débute par un clic sur la liste déroulante "*+ Ajouter…*" qui révèle les différents choix de champs possibles :

![](assets/categories/add_field_category.png)

> Il est possible de créer plusieurs sous-fiches avec différentes conditions. 

<a id="ajoutensemblechoix"></a>
### 2. Ajout d'un ensemble de choix  

Un ensemble de choix est une liste d'éléments prédéfinis permettant de remplir un champ.

> Exemple : un ensemble de choix peut consister en une liste de pays, de genre cinématographique, de professions ou de mots-clés par exemple.

Effectuer un choix permet ainsi l'affichage d'une sous-fiche dédiée. Un choix situé à n'importe quel niveau hiérarchique peut être lié à une sous-fiche.

La liste des "Ensembles de choix" est accessible en cliquant sur "Ensembles de choix" dans la barre de gauche en mode *Setup*. Une liste des ensembles de choix existants est affichée :

![](assets/choice/choice_set.png)

Il est alors possible de sélectionner un ensemble de choix existant ou d'en créer un nouveau. 

Lors de la création ou de la modification d'un ensemble de choix, il est possible de lier une sous-fiche en éditant un choix, puis en sélectionant la sous-fiche choisie sous "Sous-fiche (optionnel)".

![](assets/categories/category_choice.png)

Dans cet exemple, la **sous-fiche** *extra-data* s'affichera et permettra la saisie de données uniquement lorsque le choix *Droit* sera selectionné.

> Si la sous-fiche de s'affiche pas comme voulu: en mode *Setup*, sélectionner le type de fiche et ajouter un champ avec l'ensemble de choix avec lequel la sous-fiche est reliée.
