---
title: Éditeur de catalogue
navbar: fr-sidenav-editors.html
---

<!-- The value of title will be the h1 of the page.
The value of navbar points to the title of the sidenav file in the _include folder, to be associated with the page. Its presence or absence determines the alignment of the layout -->

<!--This is the front file. Every role has its own. Every <a> element points to a link in the navigation html file. Every <a> element is followed by the title of the content and is followed by a call to the content of the page using the include_relative syntax of Jekyll. -->

<a id="affichageajoutmod"></a>

## Affichage, ajout et modification de données

{% include_relative content/editors/affichageajoutetmodificationdedonnees.md %}

<a id="presentation"></a>

## Présentation

{% include_relative content/editors/presentation.md %}

<a id="affichagetableaux"></a>

## Affichage des tableaux de données

{% include_relative content/editors/affichagedestableauxdedonnees.md %}

## Rechercher un contenu

{% include_relative content/editors/rechercheruncontenu.md %}

<a id="ajoutdonnees"></a>

## Ajout de données

{% include_relative content/editors/ajoutdedonnees.md %}

<a id="donneesintegration"></a>

### Données d'intégration de média

{% include_relative content/editors/donneesdintegrationdemedia.md %}

<a id="donneesdatation"></a>

### Données de type datation

{% include_relative content/editors/donneesdetypedatation.md %}

<a id="donneesgeo"></a>

### Données géographiques

{% include_relative content/editors/donneesgeographiques.md %}

## Statuts des fiches

{% include_relative content/editors/statutdesfiches.md %}

<a id="editionduplsup"></a>

## Édition, duplication et suppression de fiches

{% include_relative content/editors/editionduplicationetsuppressiondefiches.md %}

<a id="suggestions"></a>

## Suggestions

{% include_relative content/editors/gestiondessuggestions.md %}

<a id="exemplecat"></a>

## Exemple d'ajout de données dans un catalogue

{% include_relative content/editors/exempledajoutdedonneesdansuncatalogue.md %}
