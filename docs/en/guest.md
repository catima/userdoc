---
title: Catalog visitor
navbar: en-sidenav-guest.html
---

A guest is a user that doesn't have a CATIMA account. The accessibility (e.g. editing items) is limited, but it is still possible to search in the catalog and view its content.

<!-- The value of title will be the h1 of the page.
The value of navbar points to the title of the sidenav file in the _include folder, to be associated with the page. Its presence or absence determines the alignment of the layout -->

<!--This is the front file. Every role has its own. Every <a> element points to a link in the navigation html file. Every <a> element is followed by the title of the content and is followed by a call to the content of the page using the include_relative syntax of Jekyll. -->

<a id="search"></a>

## Search

{% include_relative content/guest/search.md %}

<a id="advanced-search"></a>

### Advanced search

{% include_relative content/guest/advancedsearch.md %}

<a id="searchdate"></a>

### Searching the datation Field

{% include_relative content/guest/searchingthedatationfield.md %}

<a id="advancedsearchdate"></a>

#### Advanced Search

{% include_relative content/guest/advancedsearchonthedatationfield.md %}
