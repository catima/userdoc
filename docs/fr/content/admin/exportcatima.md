**Options d'export**

Dans l’export Catima, le format des données est du JSON.
Vous avez une option à choix pour cet export:
-	*Avec* ou *sans* fichiers, c’est-à-dire exporter ou pas les images et documents téléchargés dans le catalogue (*avec* étant l’option par défaut)

<!-- ![Options Catima](assets/export/export-options-catima-sql.png "Options du format JSON") -->

![Options json AND](assets/export/export-options-catima-sql.png) 

**Résultat**

Vous obtenez un dossier compressé \*.zip contenant :

1.	La **structure** des données dans le dossier *item-types*
2.	Les **données** du catalogue dans le dossier *data*
3.	(optionnel) les **fichiers** et les **images** dans le dossier *files*
4.  Les **métadonnées de l'export** (date et heure de l'export) dans le fichier *meta.json*

Ainsi que ces informations, uniquement disponibles dans l'export JSON:
- la liste des **menus** et **pages html** que vous avez définis (point 4 ci-dessous)
- les détails de **configuration** du catalogue dans le dossier *structure* (point 5 ci-dessous)

> Note: il y aura donc deux fichiers \*.json pour chaque fiche de votre catalogue; d'une part un fichier avec la structure des données, de l'autre un fichier contenant les données elles-mêmes.

![Output json AND](assets/export/export-output-json-small.png) 