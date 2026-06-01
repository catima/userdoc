
<!-- This is a FAQ front file. FAQs don't have side navigation bars. They start with a list of questions organized by themes and pointing to elements lower in the page. In the second part of the file, every content part is called under a title using the include_relative syntax of Jekyll -->

# CATIMA FAQ

Simplified documentation of [CATIMA](https://catima.github.io/userdoc/) organized in a question format.

## Adding and Editing Data

### How to create a new item type? [Read more →](#new-item-type)

### How to create conditional content? [Read more →](#conditional-content)

### How to edit the information of an existing item? [Read more →](#edit-an-item)

### How to embed media in an **item**? [Read more →](#embed-media)

### How to embed media in a **page**? [Read more →](#embed-media-in-a-page)

### How to create a custom page? [Read more →](#custom-content)

## Data Display

### How to define or change the display of an item type? [Read more →](#item-list-container)

### What sort options are available listing items? [Read more →](#data-sort)

### How to display items on a geographical map? [Read more →](#map-container)

### How to customize the catalog's navigation bar? [Read more →](#custom-navigation-bar)

## Collaboration and Access

### How to invite people and groups on a catalog? [Read more →](#invite-collaborators)

### How to restrict catalog visibility to certain members? [Read more →](#restrict-a-catalog)

### What are the different possible roles? [Read more →](#different-statuses)

## Workflow and Features

### How does the record validation system by reviewers work? [Read more →](#item-status)

<!-- ### How to create and manage a multilingual catalog?

Not in the documentation **-> to be created?** -->

### How to allow visitors of the catalog to submit comments? [Read more →](#suggestions)

----

### New item type

{% include_relative content/admin/addnewitemtype.md %}

----

### Conditional content

{% include_relative content/admin/categoriesandconditionalcontent.md %}

----

### Edit an item

{% include_relative content/editors/editduplicateanddeleteitem.md %}

----

### Embed media in an item

{% include_relative content/editors/embeddeddata.md %}

----

### Embed media in a page

{% include_relative content/admin/embedmediainacontainer.md %}

----

### Custom content

{% include_relative content/admin/createandeditcustompages.md %}

<a id="addpage"></a>

### Add a page

{% include_relative content/admin/createandeditcustompages.md %}

<a id="editpage"></a>

### Edit a page

{% include_relative content/admin/createandeditcustompages.md %}

----

### Item list Container

{% include_relative content/admin/itemlistcontainer.md %}

----

<a id="data-sort"></a>

### Sort options for Items

Sort in Catima is based on *sortable fields* of items; to be used, these fields must meet the following conditions:
- the field is readable and can be ordered logically by a human (for instance from A to Z)
- the field allows maximum one value (or can remain empty as well)

**Note**: thus, *file* or *image* fields, *geographical fields* or fields which accept multiple values cannot be sorted.

In DATA mode, these fields are rapidly identified in the list view of items. As shown below, 1) the relevant field can be selected then 2) the list shows items in *alphanumerical ascending* order (i.e. from 1 to big numbers, then from A to Z).

![champs triables AND](assets/data/data_sort_en.png) 

**Note however that**, in case you unticked the box 'Include this field in edition list view (Data)' of a field in SETUP mode, that particular field **will not show as a sort option in DATA view**, even though it meets the above conditions. It remains available elsewhere in Catima when a sort criteria can be defined.

<!-- <a href="admin.html#editionconteneurlist"> </a> -->

The same principles thus apply for instance when you add an 'ItemList' container in an HTML page.

Only *sortable fields* can be selected to define the display order: 
- By default, the sort criteria will be the primary field, provided it has been set, or the first *sortable* field of the item type. 
- For the 'line' display style, another *sortable field* can be chosen as the sort criteria

----

### Map container

{% include_relative content/admin/mapcontainer.md %}

----

### Custom navigation bar

{% include_relative content/admin/navigationbar.md %}

----

### Invite collaborators

There is a specific FAQ dedicated to the informations related to the invitation of collaborators and groups on catalog [available here](https://catima.github.io/userdoc/en/faqinvitation.html).

{% include_relative content/admin/adduser.md %}

{% include_relative content/admin/inviteuser.md %}

{% include_relative content/admin/creategroup.md %}

{% include_relative content/admin/addgroup.md %}

{% include_relative content/admin/groupid.md %}

----

### Restrict a catalog

{% include_relative content/admin/catalogaccessandvisibility.md %}

----

### Different statuses

{% include_relative content/admin/accesstodataanddataedition.md %}

----

### Item status

{% include_relative content/editors/itemstatus.md %}

----

### Suggestions

{% include_relative content/admin/suggestions.md %}

----
