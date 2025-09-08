---
title: Visiteur de catalogue
navbar: fr-sidenav-guest.html
---

<!-- The value of title will be the h1 of the page.
The value of navbar points to the title of the sidenav file in the _include folder, to be associated with the page. Its presence or absence determines the alignment of the layout -->

<!--This is the front file. Every role has its own. Every <a> element points to a link in the navigation html file. Every <a> element is followed by the title of the content and is followed by a call to the content of the page using the include_relative syntax of Jekyll. -->

## Recherche

{% include_relative content/guest/recherche.md %}

<a id="recherchesimple"></a>

### Recherche simple

{% include_relative content/guest/recherchesimple.md %}

<a id="rechercheavancee"></a>

### Recherche avancée

{% include_relative content/guest/rechercheavancee.md %}

<a id="operateurs"></a>

### Opérateurs de recherche

{% include_relative content/guest/operateursderecherche.md %}

<a id="recherchedatation"></a>

## Recherche sur le champ datation

{% include_relative content/guest/recherchesurlechampdatation.md %}
