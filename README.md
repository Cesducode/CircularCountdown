CircularCountdown
=================

Circular countdown plugin for Bootstrap

Les fichiers qui nous interessent sont circularcountdown(.min).css et circularcountdown(.min).js à placer respectivement dans les répertoires css/ et js/ de votre projet bootstrap.

Ensuite il faut les inclures dans votre page d'index.

```html
<link href="css/circularcountdown.min.css" rel="stylesheet">
...
<script src="js/circularcountdown.min.js"></script>
```
Puis ajouter la structure du compte à rebours circulaire en n'oubliant pas de renseigner dans le bloc principal `data-toggle="circularcountdown"`

```html
<div class="countdown" data-toggle="circularcountdown" data-color="belize-hole" data-to="12/25/2014">
    <div class="row">
        <div class="cdsjs col-lg-3 col-md-6 col-sm-12 col-xs-6"><canvas id="days"><!-- Days --></canvas></div>
        <div class="cdsjs col-lg-3 col-md-6 col-sm-12 col-xs-6"><canvas id="hours"><!-- Hours --></canvas></div>
        <div class="cdsjs col-lg-3 col-md-6 col-sm-12 col-xs-6"><canvas id="minutes"><!-- Minutes --></canvas></div>
        <div class="cdsjs col-lg-3 col-md-6 col-sm-12 col-xs-6"><canvas id="seconds"><!-- Seconds --></canvas></div>       
    </div>
</div>
```
Le plugin permet d'afficher pour l'instant les :

* Dixiéme de secondes -> id="tenthsec"
* Secondes  -> id="seconds"
* Minutes  -> id="minutes"
* Heures  -> id="hours"
* Jours  -> id="days"

L'exemple ci-dessus affiche les jours, heures, minutes et secondes. Le systéme de grille (col-lg, col-md...) est défini dans la division parente du canvas et s'utilise comme pour tout autre élément bootstrap.

Les paramétres à passer à CircularCountdown:
--------------------------------------------

data-to (String): La date au format mm/dd/YYYY

data-color (String): la couleur des cercles. Il est possible de renseigner une couleur prédéfini dans le plugin. On peut les retrouver sur le site [http://flatuicolors.com/](http://flatuicolors.com). Il est aussi possible de mettre les couleurs de votre choix au format hexadecimal `data-color="#3498DB"` ou au format rgb `data-color="255, 255, 255"`. A savoir que si le paramétre n'est pas renseigné, la couleur par défaut est noir.

data-fcolor (String): La couleur de la police. Les valeurs possible sont les mêmes que pour data-color.

[See example](http://htmlpreview.github.io/?https://github.com/Playntek/CircularCountdown/blob/master/index.html)

Retrouvez-nous aussi sur [Play'nTek](http://playntek.fr)

