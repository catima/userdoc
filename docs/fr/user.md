---
title: Utilisateur de catalogue
navbar: fr-sidenav-user.html
---

<!-- The value of title will be the h1 of the page.
The value of navbar points to the title of the sidenav file in the _include folder, to be associated with the page. Its presence or absence determines the alignment of the layout -->

<!--This is the front file. Every role has its own. Every <a> element points to a link in the navigation html file. Every <a> element is followed by the title of the content and is followed by a call to the content of the page using the include_relative syntax of Jekyll. -->

## Favoris

{% include_relative content/user/favoris.md %}

<a id="accescatrestreints"></a>

## Accès à des catalogues restreints

{% include_relative content/user/accesadescataloguesrestreints.md %}
