An administrator has full access to the catalog; they can add and modify any content as well as modify pages and the catalog's structure. 

# Table of contents

- [Catalog configuration](#catalog-configuration)
	- [Conceptualization](#conceptualization)
	- [Exploration](#exploration)
	- [Ranking and structure](#ranking-and-structure)
	- [Links and references](#links-and-references)
	- [Suggestions](#suggestions)
	- [Add new item type](#add-new-item-type)
	- [New field](#new-field)
	- [Field types](#field-types)
		- [Boolean field](#boolean-field)
		- [Choice set field](#choice-set-field)
		- [Date time field](#date-time-field)
		- [Decimal field](#decimal-field)
		- [Editor field](#editor-field)
		- [Email field](#email-field)
		- [Embed field (media integration)](#embed-field)
		- [File field](#file-field)
		- [Geographic field](#geographic-field)
		- [Image field](#image-field)
		- [Integer field](#integer-field)
		- [Reference field](#reference-field)
		- [Text field](#text-field)
		- [URL field](#url-field)
		- [Compound field](#compound-field)
		- [Datation field](#datation-field)
		- [Create new field](#create-new-field)
			- [Display options](#display-options)
		- [Create datation field](#createdatation)
	- [Categories and conditional content](#categories-and-conditional-content)
	- [Create and edit custom pages](#create-and-edit-custom-pages)
		- [Contact container](#contact-container)
		- [HTML container](#html-container)
		- [Item List container](#item-list-container)
		- [Map container](#map-container)
		- [Markdown container](#markdown-container)
		- [Search container](#search-container)
	- [Embed media in a page](#embed-media-in-a-container)
	- [Customize navigation bar](#navigation-bar)
	- [Statistics](#statistics)
	- [API and data only mode](#api)
	- [Catalog access](#catalog-access-and-visibility)
		- [Manage access to data](#access-to-data-and-data-edition)
		- [Change a user's status](#change-status)

<a id="catalog-configuration"></a>
# Catalog configuration

Building a new catalog is a two-step process: first, define the catalog's structure, then start to add data. This section will go over the first step; the data entry process is described in the editors section above.

<a id="conceptualization"></a>
## Conceptualization

It is important to consider the type of data that will be added to the catalog and how it will be structured before starting to add it. This reflective stage will help define catalog's conceptual and logical structure and facilitate the realization in CATIMA.  
At this stage, we are grouping different **data** together under a same **concept**.   
> For example "Titanic", "The Godfather" and "2001: A Space Odyssey" can be grouped together as "***movies***".

When there are multiple objects (or data) of one type each can have different features. To stay with the movies example, each movie has a ***Title***, ***Director***, ***Genre*** and ***Release date***. This information can be displayed in a table: 

| Title      | Genre | Director | Release date |
| ----------- | ----------- | ----------- | ----------- |
| Titanic      | Drama       | James Cameron | 1998 |
| The Godfather   | Crime        | Francis Ford Coppola | 1972 |
| 2001: A Space Odyssey   | Science-fiction      | Stanley Kubrick | 1968 |

The next steps show one way to conceptualize a dataset. 

<a id="exploration"></a>
## Exploration

Freely list all elements that will be added to the databse without worrying about any kind of order. In our example, we want to list about 20 movies.

<a id="ranking-and-structure"></a>
## Ranking and structure

We will now add some order to the list of elements. We want to find what are the important concepts and what features do they have. 
> Note: an element can be a feature of a concept and a concept as the same time: see "*Links and references*".  

In the movie example, the core concept is ***Movie*** since the catalog's goal is to list movies. But ***Director*** can also be a concept if it is considered useful to know additional features about them such as "*Date of birth*", "*Nationality*" or "*Biography*".  

<a id="links-and-references"></a>
## Links and references

Next, we will consider the relationship that each concept can have with other concepts. It is common for a concept to have a connection to one or more concepts. 
> ***Movie*** and ***Director*** have a connection as a ***Movie*** can have one or many ***Directors*** and a ***Director*** can make one or more ***Movie***. 

In CATIMA, those relationships are *References*. By adding a *Reference* field to the ***Movie*** concept about ***Director***, the ***Movie*** will appear in the ***Director*** concept.  

In CATIMA, concepts are called ***Items*** and their features ***Fields***.  

<a id="add-new-item-type"></a>
## Add new item type

After deciding which concepts and features will be used in the catalog, it is time to start adding item types. No data is added yet, this is where the item types and its fields are defined.  

First, acess the set up page by clicking on **Admin** > **Catalog set up** in the navigation bar. One must be connected to CATIMA and and be an administrator to perform this action.  

If some items have already been created, they will be displayed on the top-left of the page. Click on the "*New item type*" button to create a new one. 

![New item type](assets/setup/a-item.png)

The *New item type* form opens:

![New item type form](assets/data/new_item_type.png)

**Name**: add the item name. If different languages are selected, all fields must be completed.  
**Slug**: the slug is a short name that will appear in the website's address (URL). It must contain only letters (without accent), numbers and hyphens and must be short.  
> Example: for the item "University" the slug could be "uni".

In the **Display options**, if ***Display empty fields*** is selected, all fields will appear to the catalog's visitors, even if those are empty. If you do not wish empty fields to be shown, deselect this option. 

<a id="suggestions"></a>
## Suggestions

**Suggestions** are a way for catalog's users to send their comments to the editors and administrators. This could be used to notify about an error in a specific item. Those **Suggestions** are private and not publicly displayed on the catalog; they are sent by email to the adress defined by the administrator and are visible in data mode. 

To activate this option, select **Enable suggestions**. Unless the **Enable anonymous suggestions** is checked, only users with a Catima account can send suggestions. 

![New item type form](assets/data/setup_suggestions.png)

If suggestions are allowed for an item type, a button will appear on the top right of the screen:

![New item type form](assets/sug/item_with_suggestion.png)

When clicking, an interface will appear to write the comment:

![New item type form](assets/sug/write_suggestion.png)

When a suggestion is made, a notification is sent to the specified email adress and the suggestion is visible in data mode. A grey number ![New item type form](assets/buttons/suggestions_btn.png) next to the item indicates the number of suggestions that haven't been validated or deleted.  
They can be accessed by editing ![New item type form](assets/buttons/edit_btn.png) the item.

![New item type form](assets/sug/data_suggestions.png)

There are 3 options: 

**1**: read suggestion:  
**2**: validate suggestion: the icon will turn green and the suggestion stays visible  
**3**: delete suggestion


 ![](assets/sug/read_suggestion.png)

<a id="new-field"></a>
## New field

Once the new item created, it is time to add fields that will hold the data. Fields are the item's *features*. 

> A "*Movie*" item's fields could be a text field for the title, a date field for the release date and a choiceset field for its genre.

The number of fields an item can have isn't limited.

To add a new field to an item: 

1. On the *set up* page, select the item in the item list
2. Click on the **Add** button on the top right of the page

<a id="field-types"></a>
## Field types

In order for the catalog to be filled in by the editors with data in the right format (e.g. number, date, image), it is necessary to create appropriate fields. Here are the types of fields available in CATIMA :

<a id="boolean-field"></a>
#### Boolean field

Only for "Yes" and "No" values. 

<a id="choice-set-field"></a>
#### Choice set field

This field is for a hierarchical choice list with multiple values. It can accept a only a single selection or multiple ones. Here is an example of what the choice set field looks like when adding data:

> Note: the add ![](assets/buttons/add_btn.png) button is only available to super-editors, not simple editors.

![](assets/choice/data_choiceset.png)

The list of available **choice sets** is on the *Choices* page that is accessible from the left sidebar. Each choice can have children which can also have their own children. This allows the user to structure the choice sets. Each choice can be selected, event those that have children.

![](assets/choice/hierar_choice.png)

When a choice set is not in use anymore, there are two options: 

- **deactivate** it: this option leaves the choice set available in "Set up" but can't be used in "Data". It can be reactivated if needed.
- **delete** it: completely deletes the choice set.

<a id="date-time-field"></a>
#### Date time field

The date-time format goes from **year** only to **year, month, day, hour, minute and second**. 

<a id="decimal-field"></a>
#### Decimal field  

For decimal numbers

<a id="editor-field"></a>
#### Editor field  

Automatically displays the item's editor or the last person to modify it. 

<a id="email-field"></a>
#### Email field  

Creates a text field that only accept an email.

<a id="embed-field"></a>
### Embed field

**For media integration in a page's container, see [Embed media in a page](#embed-media-in-a-container)*

This field allows media integration such as interactive capsules, 3D models or videos to an item from websites that are independent from Catima. For the integration to be possible, the site where the media is located must be explicitly authorized explicitly by Catima. It has to be part of the **authorized domains**' list.

> e.g. to add a youtube video to an item, the domain **youtube.com** has to be authorized by Catima - which it is.

##### Non-exhaustive list of authorized domains:

- Youtube (*.youtube.com)
- Viméo (*.vimeo.com)

To know the exhaustive list of authorized domains contact the persons in charge of the project.

##### Using the embed field

In addition to the usual information such as title, slug and display options, it is also necessary to add *Additional domains* and *Format*.

![](assets/setup/embed_add_format.png)

1. **Additionnal domains**: choose form the list the authorized domains for this field. *E.g. if this field will only be for youtube video, select Youtube. But if it should be able to display videos from Youtube and Vimeo, choose both.*
 
2. **Format**: there are two ways to add a media.
	- *with iframe*: this option is to share the media only. It means that any other element on the page will not be displayed in the field. If we are embedding **Youtube** video this way, the youtube search bar, titles and comments will not be shared. Visually, this is a clean way to display a media in Catima. 
		- How to add a media in data edition mode: get the *iframe tag* from the internet page where the media currently is by clicking on **Share > Embed**. The *iframe tag* is some text that starts with `<iframe` and ends with `</iframe>`. Copy and paste it in the item's embed field.
		![](assets/setup/iframe_html.png)
		This is what it looks like when consulting the catalog:
		![](assets/setup/iframe_video1.png)
		Is it possible to add multiple medias by simply adding different *iframe tags*: 
		![](assets/setup/iframe_video2.png)
		
		> Note: due to security reasons, any other HTML tag with be deleted, the field only accepts *iframe tags*. 
		 
*with URL*: this options allows to share a complete web page with media, titles and other elements. It is convenient to use when a media can not be shared with *iframe*. Height and width can be changed, by default 400px and 900px respectively.  
> Note: it isn't always possible to use this method as the website needs to accept to be embeded this way - which sometimes is not the case. This decision is independent of Catima. E.g. Youtube and Vimeo don't allow it.
	
It is highly recommended to be specific when creating an **embed field** and add a meaninful title and/or to use *data editing help text* to let the editors know what kind of content is expected.  

<a id="file-field"></a>
#### File field  

To add external file to the item with the possibility to restrict the accepted files' type (*e.g. only .pdf and .png*). 

<a id="geographic-field"></a>
#### Geographic field  

The geographic field is used to set an item's location. It is set by drag and drop'ing a point on the map or with coordinates. It also allows to add lines and polygons to the map. In set-up mode it is possible to choose the initial zoom level i.e. how zoomed the map will be when the item is openened.
A single items can have multiple locations.

![](assets/setup/geography_zoom.png)

The field also allows to choose the colors of the polygons and the lines that will be placed on the map:

![](assets/geography/geography_colors.png)

##### Geographic fields order
Warning, if there are multiple geographic fields in the catalog, the features that use georaphic data, like the advanced search on the geographic field or the map containers, **only take into account the data stored in the first geographic field as they are positioned in the set-up.**

<a id="image-field"></a>
#### Image field  

Accepts images with optional caption.

<a id="integer-field"></a>
#### Integer field  

For integer numbers. Can also be userd to create an automatic incrementation - for exemple for id number. 

<a id="reference-field"></a>
#### Reference field  

Creates a relationship to another item. 

**E.g.** Create a reference field named *"University"* in the building item to link it to a university. This makes it so when creating a new building, it is possible to link it to a university. 

![](assets/data/ref_building.png)

This field also appears on the university item, at the bottom with a list of all buildings that are linked to it. If different items have a reference field to it, it is sorted by item type. 

![](assets/data/ref_uni.png)

<a id="text-field"></a>
#### Text field

Can be used to add short (*e.g. name or title*) or long (*e.g. description*) text. It is possible to choose between a formatted text editor or a simple text editor. 

> If this field is used as a primary field, formatted text is not possible and will be deactivated. 

<a id="url-field"></a>
#### URL field  

This field accepts URL adress and will create a link. 

<a id="compound-field"></a>
#### Compound field
The compound field allows to gather the data from other fields and to format it. It can be used to display bibliographical references. <br> The field can only be edited in *set-up mode*. It compounds the data edited in *data mode* and the result is displayed when consulting the item.

**Example** <br>
We want to list movie references in a set format. The "Movie" items contain a number of fields, including the following: "Title", "Original title", "Director", "Year of release", "Country of production".
We want to display the reference as follows.

> *Title* (Director, Country, Year).

In the compound field, choose the fields using the drop-down list and format it as required.

![](assets/compound/compound-field-en.png)

The result is displayed when consulting the item.

![](assets/compound/fiche-film-en.png)

**Multilingual catalog** <br>
The compound field can differ from one language to another. Leaving it blank in one language or the other results in a blank field. 

If the catalog is in french, we want to reference the movies in a different way. The reference should appear as follows:

> *Title* (*Original title*, Director, Year).

![](assets/compound/compound-field-fr.png)

The referece will be displayed in a different way when the catalog is in french.

![](assets/compound/fiche-film-fr.png)

> CAUTION ! If the data need to be displayed in the same way in all the language it is necessary to copy and paste the canvas in all the language allowed in the catalog.


<a id="datation-field"></a>
#### Datation field
> The datation field is a very complex field for which [a complete manual](assets/datation/exampledatation.pdf) has been produced, as well as an [example catalog](https://catima.unil.ch/datation-exple/en) showing how the field is used and how it behaves when searched.

The datation field is a field that allows for **flexible datation** of an item. It differs from the date/time field by offering the possibility of considering periods in addition to specific dates.
Searches by date can then be conducted based on a predefined period, user-defined period, or according to a specific date.

This field accepts two types of date input formats when creating new items:

- Manual entry by date/time: For each added item, input a start and/or an end of period manually.
- Choice set entry: Pre-create a choice set of *datation type* and populate it with relevant periods for the project. Then select a choice when creating the item.

> Both options can be offered for the same item type. It is possible to choose between a predefined period or to manually create one at the time of entering a new item. **However, it's not possible to input both formats in a single item.**

##### Usage Example

For a project involving an inventory of objects in a Swiss heritage building, Catima is used for referencing and dating collections. While the available information for datation of an object can sometimes be quite vague at the beginning of the process (object style, use of a technique, name of a manufacturer), as the project progresses and new documents and clues are discovered, the datation of objects becomes more precise. It's in this context that the datation choice set was designed, allowing for multiple datation clues (style, artisan, use of a technique) to be assigned. If evidence allowing for a more precise datation of an object (such as the discovery of a letter indicating the exact year of the object's creation) were to emerge , then the datation of the object could transition to manual entry to enter a specific date.

Subsequently, a person visiting the catalog will be able to search according to the datation of the recorded objects. They can search for specific dates and find objects dated to that date or including that date within the attributed period. They can search period by manually entering start and end dates or by selecting a predefined period from a choice list. They can also cross-reference periods, exclude dates, or cross-reference criteria with other fields.

##### Differences between "datation" and "date" Fields

The **date** field allows the entry of a specific date on a record. This date must be unique. It can be, for example, a person's birth date, the year of construction of a building, or the time and date of a performance.

The **datation** field accepts a start date and an end date, allowing for the creation of periods and searches on all dates contained within that period.

<a id="create-new-field"></a>
### Create a new field

A field name and slug must be chosen when creating a new field for an item:

| | Definition | Example | Note |
| ---------- | ---------- |---------- | ---------- |
| **Name** | The new field's name | *Actor's birthday* | - |
| **Name (plural)** | The new field's name - plural form | *Actors' birthdays* | - |
| **Slug** | Short and unique name | *birthday_actors* | Only accepts letters without accents and hypens. |

<a id="display-options"></a>
#### Display options 

When creating a new field, the following options can be selected:

| | Definition | Note |
| ---------- | ---------- |---------- |
| **Use this as a primary field** | This field with uniquely identify each item. It is usually a text field (Title) or integer field (ID number) | This option can only be activated for one field at a time. |
| **Include this field in edition list view (Data)** | Choose to display/not display a field in the data section. | This is useful to not display a field with a lot of informations and lighten section.|
| **Include this field in site list view** | Choose to display/not display a field to the final user when browsing all items. The field will still appear when the item is displayed, only not when all item types are listed. | Particularely useful if the item's list default is *List*. If *Grid* is selected, this option won't change anything. |
| **Restrict field to catalog staff** | Only members with invite or access to the secred code will have access to this field. | Useful to share extra information within the team that should not be displayed to the site's visitors.

<a id="createdatation"></a>
### Create a datation field

Several questions need to be addressed before starting to create a **datation** field.

1. What is the level of precision: by period, by year, by day/month/year?
2. Are the dates/periods exclusively AD (Anno Domini), or are dates/periods BC (Before Christ) also possible?
3. What input methods should be offered?
    - Manual input by date/time only (skip directly to step 2 to create the datation field)
    - Selection from a predefined set of choices (start with step 1 to configure a datation choice set before creating the datation field itself)
    - Both options (start with step 1 to configure a datation choice set)

> Field modifications are possible later on but may lead to the loss of certain data.

#### Step 1: Creating a datation choice set

This step is necessary for choosing dates through a predefined set of choices and must be done prior to creating the datation field.

In **Setup** mode, select **Choice set** from the left column and click on *+ New Choice set*. Choose the *datation* type, decide whether dates before BC are allowed or not, and select the format.

*The format and the choice set type (Date or Standard) cannot be modified once the choice set is created.*

> It's recommended to choose the widest possible format. For a datation by century, choose **Y** (years) only instead of a finer format that includes months and days, as it can lead to conflicts during searches. If date/day/month/year precision is required, choose **YMD** and do not include hours and seconds.

![](assets/datation/allowBC.png)

Edit the newly created choice set and click on *+ New Choice* to add a new period or specific date. There are several possibilities:

- The *Start Date* and *End Date* fields are filled with two different dates. They define a period from one date to another, including all dates between them.
- Only the *Start Date* field is filled. It defines a period after the indicated start date (included).
- Only the *End Date* field is filled. It defines a period before the indicated end date (included).
- Filling both fields with the same information sets a fixed date. For example, *Start Date*: 1990 and *End Date*: 1990.

![](assets/datation/bcornot.png)

> Start and end dates are **inclusive**. A period defined with a start date of **1990** and an end date of **1999** includes the years 1990, 1991, 1992, 1993, 1994, 1995, 1996, 1997, 1998, and 1999. Searching for any of these years will return records from this period.

<a id="hierarchy-choice"></a>
##### Choice hierarchy

When creating a choice, it is possible to associate a **parent** with it.
![](assets/datation/parentchoice.png)

The hierarchy of choices is visible in the **Set up** mode of the choice set. To modify the order, select the item and use the cross icon to move it to the desired location in the hierarchy. 
![](datation/hierarchie.png)

**CAUTION:** It is not recommended to create multiple levels of choice hierarchy as it can lead to confusion when searching by parent choice. During a search by choice set, children of children are not included.

**Example**
![](assets/datation/3levels.png)

- The choice 20th century
  - The choice World War II is a child of 20th century
    	- The choice year 1940 is a child of World War II

###### Impact on search

Searching for objects dated in the 20th century without including children

![](assets/datation/20thnochildren.png)

> No children are included in the search results

![](assets/datation/20thresults.png)

Searching for objects dated in the 20th century including children

![](assets/datation/20thwithchildren.png)

> The first level of children is included

![](assets/datation/20thwithresult.png)

Searching for objects dated in World War II without including children

![](assets/datation/ww2nochildren.png)

> The parent choice is no longer included

![](assets/datation/ww2noresult.png)

Searching for objects dated in World War II including children

![](assets/datation/ww2withresult.png)

> The child of the child choice is included but not the parent choice

Searching for objects dated in the 20th century including children **OR** objects dated in World War II including children

![](assets/datation/20thorww2.png)

> All 3 levels are included

![](assets/datation/20thorww2result.png)

##### In summary
The hierarchy of choices in standard or datation choice sets has a significant impact on search results. The lower in the hierarchy the choices are, the harder it becomes to find them during a search by choice set.

#### Step 2: Creating the datation field

In **Set Up** mode, select the record type from the left column and click on *+ Add > Datation Field*. In addition to the name, plural name, and slug, along with display options, the last parameter defines the format(s) used for data entry:

1. **Manual**: Check this box to allow manual entry of dates and periods. The data format is defined by selecting an option from the dropdown menu. *To enable the use of dates before BC, check the box below the dropdown menu*.
2. **Through a choice set**: Check this box and select a choice set **of date type** to allow the selection of dates or periods based on a previously created choice set. The acceptance or rejection of negative dates is defined directly in the choice set settings under *Set Up > Choice Set*.

**CAUTION!** If both input types are enabled (manual and through a choice set), it is recommended to choose the same date format.
Otherwise, ensure that you have defined **consistent** formats. The widest date format should always be included in the finer format. For example, if the choice set is in years, manual input could be in month-years format but not exclusively in months.

![](assets/datation/config_datation.png)

<a id="categories-and-conditional-content"></a>
## Categories and conditional content

An item type can have content that is common to all items (e.g. all movies have a director) but can also have conditional content (e. g. the "Period" field is relevant for *historical documentary* but not for *action movies*). It is possible to create a **category** that is displayed only if a certain **choice** is selected. In our example, the option *Period* can be show to the editor creating a new item only if the choice *Historical documentary* is displayed and otherwise hidden.  
This allows the *New item* page to remain uncluttered.  

Follow the next steps to create conditional content:  

### 1. Add a category

On the *Set up* page click on **Category > New category** in the left sidebar. It is possible to create multiple categories that are linked to different choices.  
The process of creating a new category is the same as creating a new item: chose a name and slug then add new fields.

### 2. Link it to a choice

In the left sidebar, select **Choices** and edit ![](assets/buttons/edit_btn.png) the choice set containing the choice that you want linked to the conditional content. In this example we will add conditional content to the canton *Other* in the first choice set.

![](assets/choice/a-choice-set-page.png)

Edit the choice and the last option is to add conditional content; select the category that should be displayed when that choice is selected:

![](assets/categories/a-add-category.png)

After updatation the choice, the conditional content is displayed on the right side of the choice when editing the choice set:

![](assets/categories/a-conditional-choiceset.png)

<a id="create-and-edit-custom-pages"></a>
## Create and edit custom pages

CATIMA has a default mode to display the item to the final user. This mode can not be modified, but we can create **pages** where the layout can be modified as needed.

To add a new page, click on **Pages** in the left sidebar while in *Set up* mode and click on *New page* then add a slug and title and confirm by clicking on **Create page** - or **Create and add another** if you need to add more.

![](assets/pages/a-new-page.png)

Then to modify the page, click on edit ![](assets/buttons/edit_btn.png) and the *Edit page* page will open. The slug and title can be modified and content can be added in the *Containers* section. 

> If the catalog is multilingual, there will be one container per language on the *Edit page* page. Adding an elemenet to one container doesn't automatically add it to the other ones. 

![](assets/pages/a-edit-page.png)

Different kind of content containers can be added to a page:

- **Contact**: adds a form that allows users to send an email to specified email adress. 
- **HTML**: displays a visual editor to write formatted text, links (URLs) and add images or videos. A code editor also allows advanced users to enter HTML code directly. It is this container that is used to embed media. 
- **Item List**: this container display a list of a selected item. Different styles are availables (list, grid, thumb). *Maximum one per page*
- **Map**: displays a map with a specified item type's localisation. The item must have a *Geographic field*. 
- **Markdown**: to add text, tables and images with Markdown syntax.
- **Search**: displays the results of a previously saved search. *Maximum one per page*

<a id="contact-container"></a>
### Contact container

Simply add a slug (must be unique and only letter, numbers and hypens) and an email adress. The messages will be sent directly to that specified adress.

![](assets/pages/contact_container.png)

<a id="html-container"></a>
### HTML container 

This will allow to add text, images, URL, video through a text editor. This container also allows advanced users to add pure HTML content by clicking on "Code View".
![](assets/pages/a-html-editor.png) 

> When using "Code View* it is critical to switch back to normal (by clicking the the "Code View" button again) before saving the container. If this step is skipped, the work won't be saved !

<a id="item-list-container"></a>
### Item List container

Displays all items of an item type in a list, grid, thumb or line style (e.g. to show a list of all *Universities*). Different styles are availables:

> **Note**: it is not possible to have more than one Item List container on the same page. 

![](assets/pages/item-fields.png)

After selecting a unique slug and the item type to be displayed, choose to sort the items in *ascending* or *descending* order (alphabetically), creation date or modification date. With grid, list and thumb styles the order (ascending or descending) is created based on the primary field. Whith line style, a new option appears and it is possible to choose the field to sort the items. 

> **Example**: let's say we have an item type **Book** with the following fields: *Title* (primary field), *Author*, *Publishing date* and *Illustration*. When chosing grid, list or thumb style sorting is done on *Title*. With line style it can be on *Title*, *Author* or *Publishing date*. *Illustration* will not be a possible choice as it can't be alphabetically sorted. 

#### Grid style
![](assets/pages/a-grid-style.png)

#### List style
- With images 
![](assets/pages/a-list-style.png)
- Without image
![](assets/pages/list-noimage.png)

#### Thumb style
![](assets/pages/a-thumb-style.png)

#### Line style
![](assets/pages/line-open.png)

This style displays the items vertically along a line. The user can choose to see the items in a ascending or descending order and to see all the items or none with *Close all* and *Open all*. It is then possible to only see some of the items using the small arrows.

![](assets/pages/line-closed.png)

<a id="map-container"></a>
### Map container 

The map container is used to display a geographic map of a item type that has a geographic location attribute (e.g. location of all swiss universities with geographic field). It has different options: 
	-  The item to be displayed on the map can be selected vie the **Item type** field. It will be possible to choose items that have a location attribute - items that don't have location attribute will not appear in the list:
![](assets/setup/a-map-item.png)
	- The map background can be chosen with the additional layers field. If more than one is selected, the user will be able to switch between them.
![](assets/setup/a-map-background.png)
	- The map height can be changed by changing the default height (400px) in the **Map height** attribute.
![](assets/setup/a-map-height.png)

Example of a map container:
![](assets/pages/map_container.png)

<a id="markdown-container"></a>
### Markdown container 

This container can be used to add text, images and tables with the markdown syntax. 

<a id="search-container"></a>
### Search container

![](assets/pages/search_container.png)

> **Note**: it is not possible to have more than one Search container on the same page. 
> 
Displays the result of a previously saved simple or advanced search. The "Style" settings changes the way the items are displayed. It is the same styles as listed in the [ItemList Container section](#item-list-container): Grid Style, List Style and Thumb Style. 

#### Simple search 

The simple seach bar is available on the home page. Click on the catalog's title on the top left corner to access the home page. 

![](assets/search/simple_search.png)

#### Advanced search 

With advances search, it is possible to search a specific item type and to search on one or more specific fields. The image below shows an advanced search on the item "Building", on the "Building year" field for all buildings built before the year 2000:

![](assets/search/advance_search.png)

To save a search, click on *"Save search"*. It is now in the user's profile. To see all saved searches, click on the user's email on the top right of the page (it is necessary to have a Catima account and to be connected), then *"My searches"*. From there, rename the searches is needed. That will be very useful to select the correct search for the Search container as otherwise, the title is the date and time of the search.

![](assets/search/my_searches.png)

<a id="embed-media-in-a-container"></a>
### Embed media in a container

The HTML container allows users to integrate medias such as videos, infographics and more to pages. Unlike the [embed field](#embed-field), this method allows the content to be displayed full width on the page. 

For the integration to be possible, the site where the media is located must be explicitly authorized explicitly by Catima. It has to be part of the authorized domains‘ list.

e.g. to add a youtube video to an item, the domain youtube.com has to be authorized by Catima - which it is.
Non-exhaustive list of authorized domains:

Youtube (*.youtube.com)
Viméo (*.vimeo.com)
To know the exhaustive list of authorized domains contact the persons in charge of the project.

1. Create a new or edit a HTML container and enter "Code View" mode. 
![](assets/pages/code_view.png)

2. Get the iframe tag from the internet page where the media currently is by clicking on Share > Embed. The iframe tag is some text that starts with `<iframe` and ends with `</iframe>`. Copy and paste it intot the HTML editor.
![](assets/pages/code_view_iframe.png)

3. Click on the "Code View" button again to go back to standard editing more. 
4. Save your work by clicking on the save or create container button. 

> It is critical to switch back to normal editing more before saving or creating the container with the button at the bottom of the page, otherwise the changes will be lost !

### Tip

To modify the elements' order on the page, move the blocks up or down with the arrows on the left:
![](assets/pages/a-move-container.png)

<a id="navigation-bar"></a>
## Navigation bar

The navigation bar is customizable: it is possible to add or remove items as well as change the order. To do this acces the **Menu items** settings in the left sidebar while in *Set up* mode. The current items displayed in the navigation bar are listed with their rank. An *Item type*, *Custom page* or *External URL* can be in the navigation bar. 

![](assets/menus/a-menu-items.png)

Settings can be adjusted by editing an existing item or creating a new one. Apart from the usual slug (short name that must only have small cap letters without accents, numbers or hypens) and title, the options are:

- **Rank**: change the item's order by changing its rank. The items are displayed from left to right in ascending order. 
- **Parent**: To create a drop-down menu:
	- Create a *Parent* menu item; this is the name that will appear in the navigation bar. Only fill in the slug, title and rank fields. 
	- To add *Child* menu items - options that will appear when the parent is clicked, create a new item or edit an existing one and add the *Parent* item in the parent field.   

> It is not possible for a child item to have other children.

<a id="statistics"></a>
## Statistics

The **Stats** tab in the Set up page tracks catalog's visitors. 

- The blue line is external users 
- The red one is editors and administrators on the Data and Setup page. 

![](assets/setup/stats.png)

<a id="api"></a>
## API 

Catima offers the possibility to get a catalog's informations through an API. *This option has to be activated by a system administrator. To activate your catalog's API, contact the persons in charge of the project.*

### Who can access the data ? 

One must either have a Catima account, be logged in and have access to the catalog to be able to use it's API (password method) or have the catalog's API key (API key method). The available data with the password method is the same than the data that the user has access to and can be restricted while the API key method grants access to the full catalog. For this reason, **never publicly share an API key.**

Create and delete API keys in from the **API** tab in "Set Up" mode. It is possible to have several API keys at the same time. 

More informations for API requests can be foud [in the documentation](https://catimalb.unil.ch/api-docs/index.html).

### Data only mode

A data only mode can be activated is Catima is only used to store data and a frontend catalog is not needed to access and visualize the items.

**In data only mode:**

- items can not be accessed via a catalog site by visitors
- there are no visualization options (menu, pages, visitors' statistics)
- access to data and set up mode can still be separated by role (editor, reviewer, administrator)

*This option has to be activated by a system administrator. Contact the persons in charge of the project if interested.*


<a id="catalog-access-and-visibility"></a>
# Catalog access and visibility

The CATIMA website can be accessible to all visitors or restricted to members/staff only. To configure who can see it, access the **General** setting on the left sidebar: 

![](assets/setup/a-general-setting.png)

Choose who can see your website by changing the **Catalog visibility** option:

- **Open to everyone**: the website is visible to anybody with the URL.
- **Open to members**: can be accessed by the website's members only. *To learn how to attribute member status, see Member status further down this page.*
- **Open to catalog staff**: the catalog is only accessible my *editors*, *super-editors*, *reviewers* and *administrators*. 

Other options are accessible from this page:

- **Name**: change the name of the website
- **Advertize**: by checking it, your catalogue will be accessible from public CATIMA lists.
- **Custom root page**: change the landing page 

<a id="access-to-data-and-data-edition"></a>
## Access to data and data edition 


CATIMA has different staus that can be attributed to users; those status define what a user can or can't do within a given catalog. Guests are users that don't have a CATIMA account and must create one to have access to other status.

> Status are catalog specific and a user can have different status in different catalogs. 

**Users** can view the public areas of the non-restricted catalogs.  
**Members** are users that can view the public areas of a restricted catalog.  
**Editors** are members that can create and edit their own items in the catalog.  
**Super-editors** are editors that can create and edit all the items in the catalog and add new choice in choice sets.
**Reviewers** validate itesm created by **editors** and **super-editors**.
**Administrator** have access to all the catalog's options. 

<a id="change-status"></a>
## Change status

It is possible to invite people to see a private catalog or colaborate by changing their status. They will get an email with the invite. To edit a user's status, got to **Users & groups** in the left sidebar on the "Set up" page.

Status can be changed in two ways: 

1. One person at a time: search for the user and click on edit ![](assets/buttons/edit_btn.png). After selcting a prefered language, their status can be updated. 
2. Use the *Group* setting: add a new group, give it a name and description.

![](assets/groups/a-new-group.png) 

If the "Public" checkbox is not checked, only members with an email invitation are part of the group. To add members to the group with email adresses, click on the ![](assets/groups/usergroup_icon.png) icon. 

If the "Public" checkbox is checked, CATIMA will create a password that can be shared with anybody. This pasword is the key to be part of the group. 
> To generate the password, check the "Public" checkbox, update the group and edit it again.

Users can also be given editor or super-editor status the same way.

> Users won't be able to see the catalog if its visibiliy is set on *Open to members* or *Open to catalog staff.
> Members won't be able to see the catalog if its visibility is set on *Open to catalog staff*.
> To change the catalog's visibility, go to *Set up > General > Catalog visibility*
