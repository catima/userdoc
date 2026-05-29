**Options**

In the Catima export, the format is JSON.
You can chose to export the complete catalog data:
-	*With* ou *without* files, i.e. export images and document files as well (*with* is the default  option)

![JSON Options AND](assets/export/export-options-catima-sql-en.png) 

**Results**

The \*.zip folder contains :

1.	The data **structure** in folder *item-types*
2.	The catalog **data** in folder *data*
3.	(optionnal) the **files** and **images** in folder *files*
4.  The **export metadata** (i.e. date and time of the export) is found in file *meta.json*

As well as the below information, which is only available in the JSON export:
- the list of **menus** and **HTML pages** that you defined (point 4 below)
- the **configuration** details of the catalog in folder *structure* (point 5 below)

> Note: for every *item type* you will obtain two \*.json files; the data structure is described in json files contained in the folder *item-types*, the data itself is contained in json files of the *data* folder.

![JSON Output AND](assets/export/export-output-json.png) 