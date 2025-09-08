---
title: Catalog user
navbar: en-sidenav-user.html
---
CATIMA's catalog users and people that have a CATIMA account and are connected. While connected, it is possible to add content to the favorites.

<!-- The value of title will be the h1 of the page.
The value of navbar points to the title of the sidenav file in the _include folder, to be associated with the page. Its presence or absence determines the alignment of the layout -->

<!--This is the front file. Every role has its own. Every <a> element points to a link in the navigation html file. Every <a> element is followed by the title of the content and is followed by a call to the content of the page using the include_relative syntax of Jekyll. -->

<a id="favorites"></a>

## Favorites

{% include_relative content/user/favorites.md %}

<a id="access-restricted-catalogs"></a>

## Access restricted catalogs

{% include_relative content/user/accessrestrictedcatalogs.md %}
