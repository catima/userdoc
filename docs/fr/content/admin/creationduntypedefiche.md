Un catalogue permet de stocker des données (texte, images, dates, etc...) structurées sous la forme de types de fiches. Les types de fiches représentent des entités conceptuelles (p.ex le concept "livre") possédant des caractéristiques définies (p.ex "auteur", "année de publication").

Dans CATIMA les concepts sont appelés "**Types de fiches**" et leurs caractéristiques des **Champs**.

Pour accéder à la section de configuration ("Setup"), cliquer sur "Admin" dans la barre horizontale supérieure, puis choisir "Catalog Setup" dans le menu déroulant. Une interface résumant les éventuels objets existants s'affiche.

Pour ajouter un objet, cliquer sur "+ Nouveau type de fiche" en bas de la rubrique "Types de fiche", dans la barre latérale gauche. 

![](assets/setup/new_item_type1.png)

Le formulaire suivant s’affiche :

![](assets/setup/new_item_type2.png)

Remplir le nom du type de fiche et sa forme plurielle. Si le support de plusieurs langues a été demandé pour le catalogue, il s'agira de remplir également ces éléments traduits dans les autres langues. Pour terminer, choisir une forme simplifiée du nom appelée "slug" qui apparaitra dans l'adresse web (URL) du site généré par CATIMA. Celui-ci doit être unique et n'être composé que de lettres (non accentuées), nombres et de traits d'unions. Les slugs sont souvent en anglais.

> Exemple : Pour un type de fiche "Acteurs de films", le slug peut être "movies-actors"

Si l'option **Afficher les champs vides** n'est pas sélectionnée, les champs qui ne contiennent aucune données ne seront pas vu par les visiteurs du catalogue. 