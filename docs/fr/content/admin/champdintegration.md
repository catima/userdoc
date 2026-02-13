*Pour l'intégration de média à une page, voir la rubrique [Intégration de média (embed) dans une page](#integrationmediapage).*

Ce champ permet l'intégration de médias tels que des capsules interactives, des modèles 3D ou des vidéos à une fiche à partir de sites web indépendants de Catima.  Pour que l'intégration soit possible, il faut que le site sur lequel le média se trouve soit explicitement autorisé par Catima. Il doit faire partie de la **liste des domaines autorisés**.  

> Exemple: afin de pouvoir publier une vidéo youtube dans une fiche, il faut que le domaine **youtube** soit autorisé par Catima - ce qui est le cas.

##### Liste non-exhaustive des domaines autorisés:

- Youtube (*.youtube.com)
- Viméo (*.vimeo.com)

Pour connaître la liste exhaustive des domaines autorisés (qui peut évoluer en fonction des besoins), se référer aux personnes responsables. 

##### Utilisation du champ d'intégration (embed) 

En plus des informations standards telles que nom, slug et options d'affichage, il faut aussi spécifier les *domaines supplémentaires* et le *format voulu*. 

![](assets/setup/integration.png)

1. **Domaines supplémentaires**: choisir dans cette liste les domaines autorisés pour ce champ. *Par exemple: si le champ est uniquement pour des vidéos provenant de youtube, sélectionner Youtube. Mais si le champ est pour des vidéos provenant de youtube et/ou viméo, sélectionner Youtube et Viméo.*

2. **Format voulu:** il est possible d'intégrer le média de 2 façons différentes. 
	- *Par iframe*: cette option est pour partager un média uniquement. Les autres éléments présents sur la page ne sont pas pris en compte. Dans le cas de **Youtube**, iframe permet de partager uniquement la vidéo sans la barre de recherche youtube, le titre, les commentaires et tous les autres éléments autour. Cette option permet généralement un intégration plus propre. Un *iframe* est un simple bout de texte. 
		- Pour intégrer un média à une fiche avec iframe en mode édition (Data): récupérer la *balise iframe* depuis la page internet où se trouve le média en cliquant sur le bouton ou l'option **Partager (ou Share)** > **Embed**. Le texte en question commence par `<iframe` et se termine par `</iframe>`. Le et le coller dans le champ d'intégration de la fiche:
![](assets/setup/integration_iframe.png)
Résultat lors de la consultation de la fiche:
![](assets/setup/integration_youtube.png)
Pour ajouter plus d'un média, il est possible d'insérer plusieurs balises iframe l'une après l'autre:
![](assets/setup/integration_mult.png)  

> *Note: Pour des raisons de sécurité, le champ intégration supprime toutes autres balises et garde uniquement la balise iframe.*  

***Par URL***: cette option permet de partager une page d'un site internet avec la mise en page, les titres et autre éléments. Ceci est surtout pratique quand un site ne propose pas d'option de partage par iframe. La largeur et la hauteur sont personnalisables - par défaut 900px et 400px.   
> Attention: il n'est pas toujours possible d'intégrer des pages de cette manière car il faut que le site en question accepte d'être intégré par URL. Cette décision est indépendante de Catima. Par exemple, Youtube et Viméo ne permettent pas de le faire.

Lors de la création d'un **champ d'intégration (embed)**, il est vivement conseillé de créer un titre explicite spécifiant le type d'intégration tel que *Intégration par iframe* et *Intégration par url* ou d'ajouter un texte d'aide à la saisie afin que les personnes ajoutant du contenu au catalogue sachent quel contenu ajouter.

##### Intégration avec dilps et tiresias

Pour permettre l'intégration de fiches provenant des bases de données [dilps.unil.ch](https://dilps.unil.ch/home) et [tiresia.unil.ch](https://tiresias.unil.ch/home) il faut choisir le type d'intégration **url** et ne pas oublier d'autoriser le ou les domaines concernés dans la liste des domaines autorisés.

![](assets/data/allow-domains.png)

> Attention à ne pas changer le type d'intégration d'un champ déjà existant  au risque de perdre les intégration préalablement ajoutées dans les données. Si un nouveau type d'intégration est nécessaire, créer un nouveau champ d'intégration en précisant le type d'intégration dans le titre.