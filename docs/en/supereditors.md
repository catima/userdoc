---
title: Catalog super-editor
navbar: en-sidenav-supereditors.html
---

A super-editor can add and edit any item as well as add choices to existing choice sets.

<!-- The value of title will be the h1 of the page.
The value of navbar points to the title of the sidenav file in the _include folder, to be associated with the page. Its presence or absence determines the alignment of the layout -->

<!--This is the front file. Every role has its own. Every <a> element points to a link in the navigation html file. Every <a> element is followed by the title of the content and is followed by a call to the content of the page using the include_relative syntax of Jekyll. -->

<a id="add-new-choice-to-choice-set"></a>

## Add new choice to choice set

{% include_relative content/supereditors/addnewchoicetochoiceset.md %}

<a id="addperiodchoice"></a>

## Add new period to a datation choice set

{% include_relative content/supereditors/addnewperiodtoadatationchoiceset.md %}

<a id="choicehierachy"></a>

## Choice hierarchy

{% include_relative content/supereditors/choicehierarchy.md %}
