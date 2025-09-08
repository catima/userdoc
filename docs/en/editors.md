---
title: Catalog editor
navbar: en-sidenav-editors.html 
---

A catalog's editor can view the website and add new items/content to it, but not modify pages and structure.

<!-- The value of title will be the h1 of the page.
The value of navbar points to the title of the sidenav file in the _include folder, to be associated with the page. Its presence or absence determines the alignment of the layout -->

<!--This is the front file. Every role has its own. Every <a> element points to a link in the navigation html file. Every <a> element is followed by the title of the content and is followed by a call to the content of the page using the include_relative syntax of Jekyll. -->

<a id="display-items"></a>

## Display items

{% include_relative content/editors/displayitems.md %}

<a id="add-item"></a>

## Add item

{% include_relative content/editors/additem.md %}

<a id="embed-data"></a>

### Embendded Data

{% include_relative content/editors/embeddeddata.md %}

<a id="datationdata"></a>

### Datation Data

{% include_relative content/editors/datationdata.md %}

<a id ="geographicdata"></a>

### Geographic data

{% include_relative content/editors/geographicdata.md %}

<a id="item-status"></a>

## Item status

{% include_relative content/editors/itemstatus.md %}

<a id="suggestions"></a>

## Suggestions

{% include_relative content/editors/suggestions.md %}

<a id="editduplicatedelete"></a>

## Edit, duplicate, and delete item

{% include_relative content/editors/editduplicateanddeleteitem.md %}
