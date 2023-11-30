Ce type de *conteneur*, permet d'afficher (sur la page personnalisée) toutes les données enregistrées dans un type de fiche donné ainsi que de changer le style d'affichage des fiches (aperçu d'images, grille, liste ou line).

> **Attention**: il n'est pas possible d'avoir plus d'un conteneur *Item List* par page.

 ![](assets/pages/itemlist-fields.png)

Choisir un "slug" (nom court à donner au conteneur). Celui-ci apparaitra dans l'adresse web (URL) du site généré par CATIMA. Il doit être unique et n'être composé que de lettres (non accentuées), nombres et de traits d'unions. Les slugs sont souvent en anglais.

> **Exemple de slug**: "liste-oeuvres", "work-list", "img-gallery"

Choisir aussi un ordre d'affichage *ascendant* ou *descendant*, par champ, date de création ou date de modification. Dans le cas des affichages par images, grille ou liste, le champ sélectionné est le champ primaire. Pour l'affichage de type line, il est possible de sélectionner le champ voulu parmis la liste de champs disponibles.

> **Exemple en mode line**: nous avons un type de fiche *Livre* qui contient les champs *Titre* (champ primaire), *Auteur*, *Date de publication* et *Image*. Le tri des fiches se fera selon le *Titre* (champ primaire) en mode images, gille ou liste. En mode line, il est possible de choisir de faire le tri selon le *Titre*, l'*Auteur* ou la *Date de publication*. Comme il n'est pas possible de classifier des image d'une manière ascendante (ou descendante), ce champ n'est pas sélectionnable pour le tri.  

Le choix du style permet de changer l'affichage des fiches selon les styles suivants : 

<a id="images-thumb"></a>
#### Images (thumb):
![](assets/pages/style-thumb.png)

<a id="grille-grid"></a>
#### Grille (grid):
![](assets/pages/style-grid.png)

<a id="liste-list"></a>
#### Liste:
 - Avec image:  
 ![](assets/pages/style-list-img.png)
 - Sans image:  
 ![](assets/pages/style-list-text.png)
 
<a id="ligne-line"></a>
#### Ligne (line):
![](assets/pages/style-list-line-open.png)

Le style *line* affiche les fiches le long d'une ligne verticale; il permet le tri par date ou ordre alphabétique. Le visiteur peut ouvrir ou fermer les fiches et les classer par ordre ascendant ou descendant. Dans l'image ci-dessous, on a choisi *Tout fermer* avant d'ouvrir une seule fiche.

![](assets/pages/style-list-line-closed.png)