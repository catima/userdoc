**For media integration in a page's container, see [Embed media in a page](#embed-media-in-a-container)*

This field allows media integration such as interactive capsules, 3D models or videos to an item from websites that are independent from Catima. For the integration to be possible, the site where the media is located must be explicitly authorized explicitly by Catima. It has to be part of the **authorized domains**' list.

> e.g. to add a youtube video to an item, the domain **youtube.com** has to be authorized by Catima - which it is.

##### Non-exhaustive list of authorized domains

- Youtube (*.youtube.com)
- Viméo (*.vimeo.com)

To know the exhaustive list of authorized domains contact the persons in charge of the project.

##### Using the embed field

In addition to the usual information such as title, slug and display options, it is also necessary to add *Additional domains* and *Format*.

![i](assets/setup/embed_add_format.png)

1. **Additionnal domains**: choose form the list the authorized domains for this field. *E.g. if this field will only be for youtube video, select Youtube. But if it should be able to display videos from Youtube and Vimeo, choose both.*

2. **Format**: there are two ways to add a media.
   - *with iframe*: this option is to share the media only. It means that any other element on the page will not be displayed in the field. If we are embedding **Youtube** video this way, the youtube search bar, titles and comments will not be shared. Visually, this is a clean way to display a media in Catima.
     - How to add a media in data edition mode: get the *iframe tag* from the internet page where the media currently is by clicking on **Share > Embed**. The *iframe tag* is some text that starts with `<iframe` and ends with `</iframe>`. Copy and paste it in the item's embed field.
		![i](assets/setup/iframe_html.png)
		This is what it looks like when consulting the catalog:
		![i](assets/setup/iframe_video1.png)
		Is it possible to add multiple medias by simply adding different *iframe tags*:
		![i](assets/setup/iframe_video2.png)

		> Note: due to security reasons, any other HTML tag with be deleted, the field only accepts *iframe tags*.

*with URL*: this options allows to share a complete web page with media, titles and other elements. It is convenient to use when a media can not be shared with *iframe*. Height and width can be changed, by default 400px and 900px respectively.  
> Note: it isn't always possible to use this method as the website needs to accept to be embeded this way - which sometimes is not the case. This decision is independent of Catima. E.g. Youtube and Vimeo don't allow it.

It is highly recommended to be specific when creating an **embed field** and add a meaninful title and/or to use *data editing help text* to let the editors know what kind of content is expected.

##### Embed dilps et tiresias pages

To allow the embedding of pages from the dilps.unil.ch or tiresias.unil.ch databases it is necessary to choose the **url** format and to not forget to select the relevant domains in the allowed domains list.

![](assets/data/allow-domains.png)

> Be careful not to change the format of an existing embed field to avoid loosing embeds previously logged in the data. If having a new format is necesssary, create a new embed field with a title stating clearly the type of format it allows.