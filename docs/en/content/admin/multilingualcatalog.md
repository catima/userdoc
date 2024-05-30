
It is possible to configure Catima in French, English, German, or Italian. Catima also allows the creation of multilingual catalogs, enabling users to switch between languages while browsing the catalog. However, multilingual catalogs involve a number of parameters to consider. It is therefore recommended to read this documentation carefully.

> Warning! Catima interfaces in **set-up and data** mode and the **documentation** are only available in French and English. If the catalog is configured in German or Italian, the default language will be English.

![](assets/multilingual/choose_language.png)

### Creating a Multilingual Catalog

The language of a catalog is generally defined at the time of its creation and communicated to the member of the Catima team in charge of your catalog. Any addition or change of language after the catalog is created must be carried out by the administrators of Catima. It is not recommended to add a language to an existing catalog as this involves a number of complications and translation work for the catalog's staff.

In multilingual catalogs, the names of each item type as well as the names of each field must be translated into all the languages of the catalog. The choices of [choice sets](#choice-set-field) and [datation choice sets](#step-1-creating-a-datation-choice-set) must also be translated. Slugs are always unique, English is conventionally preferred.

<a id="multilingual-fields"></a>

The following field types can be configured as multilingual:

#### Text Field and URL Field

When the multilingual option is enabled, provided the field is not the primary field, editors can enter data in one or more of the catalog's languages. If a language is not filled in, the field will not appear when viewing the record in the missing language.

**If the field is defined as the primary field, it must be filled in all the catalog's languages.**

#### Compound Field

The compound field can only be modified by the catalog administrators. The formatting in each language is defined in the *Set-up* mode of the field according to [the documentation related to this field](#compound-field-1).

### Adding a Language to an Existing Catalog

Adding a language after the creation of a catalog is strongly discouraged. However, if it is necessary to add a language, refer to the Catima managers. To add a new language to an already conceptualized catalog containing existing data, follow these steps:

* Schedule a meeting with the Catima managers to discuss your decision and implement the change
* Translate the names of each record type into the added language
* Translate the names of **each field in each record type**
* Enable or not the multilingual option in the [relevant fields](#multilingual-fields).
* Translate **all choices** in the [choice sets](#choice-set-field) and [datation choice sets](#step-1-creating-a-datation-choice-set)
* Then switch to data mode and edit **all existing items** to translate the multilingual data in the [relevant fields](#multilingual-fields).

> Warning! Skipping any of these steps may result in possible data loss when viewing the catalog depending on the chosen language.
