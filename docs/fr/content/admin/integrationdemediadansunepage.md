Il est possible d'intégrer des médias tels que des vidéos, des capsules interactives ou des modèles 3D dans une page avec le conteneur HTML. **L'intégration (embed) dans une *page*** permet un affichage sur toute la page si cela est souhaité. 

Noter la différence: **L'embed des *fiches*** ne permet pas un affichage pleine page; pour ceci, se référer à la partie traitant du [champ d'intégration (embed) de la fiche](#champintegration). 

Pour que **l'intégration (embed) dans une page** soit possible, il faut que le site sur lequel le média se trouve soit explicitement autorisé par Catima. Il doit faire partie de la **liste des domaines autorisés**.  

> Exemple: afin de pouvoir publier une vidéo youtube dans une fiche, il faut que le domaine **youtube** soit autorisé par Catima - ce qui est le cas.

##### Liste non-exhaustive des domaines autorisés:

- Youtube (*.youtube.com)
- Viméo (*.vimeo.com)

Pour connaître la liste exhaustive des domaines autorisés (qui peut évoluer en fonction des besoins), se référer aux personnes responsables. 

1. Créer ou éditer un conteneur HTML et entrer en mode "Code View".
 	![](assets/pages/code_view.png)
2. Récupérer la *balise iframe* depuis la page internet où se trouve le média en cliquant sur le bouton ou l'option **Partager (ou Share)** > **Embed**. Coller et copier le texte dans le conteneur HTML. Le texte en question commence par `<iframe` et se termine par `</iframe>`. 
   ![](assets/pages/code_view_iframe.png)
3. Retourner en mode d'édition normal pour visualiser le résultat. Cette étape est nécessaire pour sauvegarder le travail. 
4. Sauvegarder avec *"Créer conteneur"* ou *"Enregistrer conteneur"*.

> Il est possible de personnaliser l'affichage du conteneur en ajoutant du code HTML en plus de la balise iframe.  