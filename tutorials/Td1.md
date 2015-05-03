---
title: Programmation Web - Client Riche
layout: main
---

# Td1 -- Javascript et callbacks

## Les outils de développements

Nous allons utiliser les outils de développements de Chrome pour nos Tds. 
Pour ouvrir les outils de développements de Chrome, appuyez sur `F12` (ou `Ctrl+Shift+I` ou Onglet Outils > Outils de développement).

#### L'inspecteurs d'éléments de page Web 

L'onglet **Élément** contient le code HTML de la page Web courante.
En survolant le code HTML, l'inspecteur vous indique où se trouve la boîte englobant l'élement courant. Les rectangles affichés de couleurs différentes représentent les quatres boites englobantes : la marge extérieure (`margin`), la bordure, la marge intérieure (`padding`) et le contenu.

Les dimensions des boîtes sont indiquées dans l'onglet style, qui regroupe toutes les règles CSS s'appliquant à cet élément.

À l'inverse, vous pouvez vous servir de la loupe ![loupe]({{ site.baseurl }}/assets/magnifying.png) pour explorer visuellement le rendu de la page Web. La loupe vous montre alors le code HTML de l'élément sous votre souris.

<div class="exercice">
1. Inspectez la page courante dans l'onglet **Élément**. 
  * Éditez la page HTML. Modifiez le texte du TD. Rajouter ou enlevez des balises de la page HTML. <br/>
**Note:** Pour éditer le HTML, il faut faire clic droit > 'Edit as HTML'.
  * Changez des éléments de style, par exemple la façon dont les bouts de code en ligne (e.g. `margin`, `padding`) sont stylisés. Ou passez à une numérotation binaire des listes d'exercices (`list-style-type: binary` - [Ne marche pas sur Firefox ni IE](http://www.quirksmode.org/css/lists.html)).
  * Rajouter votre premier gestionaire d'évènement (event handler)
</div>

Les modifications que vous avez faites sont temporaires et disparaîtrons lors du rechargement de la page. Il faudrait reporter les modifications côté serveur pour les enregistrer.

#### Le moniteur réseau

L'onglet **Network** permet d'observer les requêtes HTTP faites pour charger votre page. On y voit le chargement de la page HTML, des styles CSS et des images liées.

<div class="exercice">
1. Cliquez sur la ligne de la page Web *Td1.html* et observez l'onglet **Headers**. On y voit les caractéristiques principales de la requête HTTP qui demande la page au serveur :
  * l'adresse du serveur : **romainlebreton.github.io**
  * l'url de la page demandée : **http://romainlebreton.github.io/ProgWeb-ClientRiche/tutorials/Td1.html**
  * la méthode de requête : **GET**
  * le code de status de la réponse : 200 OK ou 304 Not modified (ou 404 Not Found)
</div>

#### La console Javascript

C'est ici que nous allons passer le reste du Tds. L'onglet **Console** présente deux avantages :
1. c'est une console Javascript. Ce sera donc notre bac à sable pour expérimenter du code Javascript;
2. nous avons accès au DOM de la page Web courante. Ceci nous permettra d'interagir avec la page Web. Nous y reviendrons bientôt.




### Sources

- [La présentation des outils de développements sur le site de Chrome](https://developer.chrome.com/devtools)