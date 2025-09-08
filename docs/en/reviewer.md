---
title: Catalog reviewer
navbar: en-sidenav-reviewer.html
---

A reviewer can approve or reject an item created by (super-)editors.

<!-- The value of title will be the h1 of the page.
The value of navbar points to the title of the sidenav file in the _include folder, to be associated with the page. Its presence or absence determines the alignment of the layout -->

<!--This is the front file. Every role has its own. Every <a> element points to a link in the navigation html file. Every <a> element is followed by the title of the content and is followed by a call to the content of the page using the include_relative syntax of Jekyll. -->

<a id="status"></a>

## Status

{% include_relative content/reviewer/status.md %}

<a id="workflow"></a>

## Workflow

{% include_relative content/reviewer/workflow.md %}

<a id="approve-or-reject-an-item"></a>

## Approve or reject an item

{% include_relative content/reviewer/approveandrejectanitem.md %}
