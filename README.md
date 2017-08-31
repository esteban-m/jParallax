# jParallax
Plugin jQuery pour faire des parallax de type rigolo qui marche avec le mouvement de ton curseur de ton ordinateur informatique adapté à l'internet du web !

## Installation

Alors déjà faut mettre jQuery, si tu connais pas... C'est problématique, va sur Google et reviens !

`<script src="https://cdnjs.cloudflare.com/ajax/libs/jquery/3.2.1/jquery.min.js"></script>`

Ah ! T'as trouvé c'est quoi jQuery ? Bon nickel ! Maintenant faut installer le plugin.. Quoi ? Tu connais pas c'est quoi un plugin ? Bon, va voir sur Google et reviens.

`<script src="js/jParallax.js"></script>`

On va y arriver, bon maintenant tes éléments que tu veut voir bouger, donne leur une classe en Hache TML.

`<div class="bg1"></div>`

`<div class="bg2"></div>`

`<div class="bg3"></div>`

`<div class="bg4"></div>`

T'es la ? Non.. Mais reviens c'est presque fini ! Un dernier truc, il te reste plus qu'à déclarer tes éléments !

`	$('.bg1').mouseParallax({ moveFactor:  5, targetContainer: '.parallax' });`

`	$('.bg2').mouseParallax({ moveFactor: 10, targetContainer: '.parallax' });`

`	$('.bg3').mouseParallax({ moveFactor: 15, targetContainer: '.parallax' });`

`	$('.bg4').mouseParallax({ moveFactor: 20, targetContainer: '.parallax' });`

## Explication

Je t'explique vite fait c'est quoi tout ça !

`$('.bg1')` Ce truc c'est la classe de ton élément, t'as le droit de mettre aussi un ID `.mouseParallax` Bon ça c'est la fonction qui fait tout le truc `({ moveFactor:  5` La c'est un facteur d'amplitude, 5 c'est la valeur par défaut si tu le met pas, met un chiffre plus gros et ton élément se déplacera plus vite ! `, targetContainer: '.parallax' });` dernier paramètre, c'est le conteneur, le parent des éléments, par défaut c'est body donc pareil t'es pas obligé de le mettre.

## Credit

Le plugin original c'est celui la : http://www.jqueryscript.net/animation/Interactive-Mouse-Hover-Parallax-Effect-with-jQuery-Mouse-Parallax.html

Je l'ai modifié pour qu'il fonctionne avec le paramètre translate en CSS, ça le rend compatible avec beaucoup plus d'éléments comme le SVG par exemple !
