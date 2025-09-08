---
title: Super-éditeur de catalogue
navbar: fr-sidenav-supereditors.html
---

<!-- The value of title will be the h1 of the page.
The value of navbar points to the title of the sidenav file in the _include folder, to be associated with the page. Its presence or absence determines the alignment of the layout -->

<!--This is the front file. Every role has its own. Every <a> element points to a link in the navigation html file. Every <a> element is followed by the title of the content and is followed by a call to the content of the page using the include_relative syntax of Jekyll. -->

En plus de la création de nouvelles fiches, un super-éditeur peut modifier toutes les fiches existantes et ajouter des choix dans les ensembles de choix.

<a id="ajout-choix"></a>

## Ajout de choix dans les ensembles de choix

{% include_relative content/supereditors/ajoutdechoixdanslesensemblesdechoix.md %}

<a id="ajoutchoixdatation"></a>

## Ajouter des choix dans les ensembles de choix de type datation

{% include_relative content/supereditors/ajoutdeschoixdetypedatation.md %}

<a id="choixparents"></a>

## Choix parents et choix enfants

{% include_relative content/supereditors/choixparentsetchoixenfants.md %}
