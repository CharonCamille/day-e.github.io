# Jour 5

## <a href="https://joz84.github.io/day-e.github.io/" target="_blanck">Demo</a>

## <a href="https://mailchimp.com/" target="_blanck">MailChimp</a>

<a href="https://mailchimp.com/" target="_blanck">MailChimp</a> est un service en ligne qui permet de gérer des envoies de mails groupés. Il faut créer un "audience" (liste de mails destinataire de la future newsletter), un "template" (email type contenant la newletter) et enfin une "campagne" qui est l'action d'envoyer un template à une audience. 

Vous trouverez ici les imprim-écrans des différentes étapes à suivre pour intégrer un formulaire d'inscription à une audience (newsletter <a href="https://mailchimp.com/" target="_blanck">MailChimp</a>) :

<a href="https://docs.google.com/presentation/d/e/2PACX-1vRQPuy_5olP8j4p9P2KbDMsO_igLcq2mOWLcCuHNX7YECwDOi7e0WnyA1XM-8E1sDXk9dHxTcGE9E2g/pub?start=false&loop=false&delayms=3000" target="_blanck">Mailchimp demo</a>

Une fois le code d'intégration récupérer, il doit être collé là où l'on souhaite voir apparaitre le formulaire. On remarque que le code récupérér contient 3 parties : un lien vers une page de CSS (balise "link"), le formulaire et du JS (balises "script). Par souci de clartée nous avons séparré ces trois bouts de codes:

### Le lien vers la page CSS (balise "link") (l.8)
Les links se mettent toujours dans le head avant le link vers sa propre page de stye (style.css)

```html
<link href="https://cdn-images.mailchimp.com/embedcode/classic-10_7.css" rel="stylesheet" type="text/css">
```  
### Le formulaire (l.147-176)
```html
      <!-- Begin Mailchimp Signup Form -->
      <div id="mc_embed_signup">
        <form action="https://a-waree.us15.list-manage.com/subscribe/post?u=9ef09dfae3eb2da317e4e3b49&amp;id=acb7df8fb7" method="post" id="mc-embedded-subscribe-form" name="mc-embedded-subscribe-form" class="validate" target="_blank" novalidate>
          <div id="mc_embed_signup_scroll">
            <h2 class="color-green">Souscrire à notre newsletter</h2>
          <div class="indicates-required"><span class="asterisk">*</span> indicates required</div>
          <div class="mc-field-group">
            <label for="mce-EMAIL">Email<span class="asterisk">*</span></label>
            <input type="email" value="" name="EMAIL" class="required email" id="mce-EMAIL">
          </div>
          <div class="mc-field-group">
            <label for="mce-FNAME">Nom de famille</label>
            <input type="text" value="" name="FNAME" class="" id="mce-FNAME">
          </div>
          <div class="mc-field-group">
            <label for="mce-LNAME">Prénom</label>
            <input type="text" value="" name="LNAME" class="" id="mce-LNAME">
          </div>
          <div id="mce-responses" class="clear">
            <div class="response" id="mce-error-response" style="display:none"></div>
            <div class="response" id="mce-success-response" style="display:none"></div>
          </div>
          <div style="position: absolute; left: -5000px;" aria-hidden="true"><input type="text" name="b_9ef09dfae3eb2da317e4e3b49_acb7df8fb7" tabindex="-1" value=""></div>
            <div class="clear">
              <input type="submit" value="Souscrire" name="subscribe" id="mc-embedded-subscribe" class="btn-pink">
            </div>
          </div>
        </form>
      </div>
      <!--End mc_embed_signup-->
```

### Le JS (l.230-247)
Le javascript se met toujours à la fin avant </body>
```html
  <script type='text/javascript' src='//s3.amazonaws.com/downloads.mailchimp.com/js/mc-validate.js'></script>
  <script type='text/javascript'>
    (function($) {
      window.fnames = new Array();
      window.ftypes = new Array();
      fnames[0]='EMAIL';
      ftypes[0]='email';
      fnames[1]='FNAME';
      ftypes[1]='text';
      fnames[2]='LNAME';
      ftypes[2]='text';
      fnames[3]='ADDRESS';
      ftypes[3]='address';
      fnames[4]='PHONE';
      ftypes[4]='phone';
    }(jQuery));
    var $mcj = jQuery.noConflict(true);
  </script>
```


## <a href="https://www.typeform.com/" target="_blanck">TypeForm</a>

<a href="https://www.typeform.com/" target="_blanck">TypeForm</a> est un service en ligne qui permet de créer des formulaires et de les partager en ligne.

Vous trouverez ici les imprim-écrans des différentes étapes à suivre pour intégrer un formulaire <a href="https://www.typeform.com/" target="_blanck">TypeForm</a> :

<a href="https://docs.google.com/presentation/d/e/2PACX-1vRUaC-lrvdei4Qb1gCEdE6kIRB677I-Nys0QlpK-JlUUTRT4WijsrSXz4p__PNqAY0_OuVoWA6cCWwy/pub?start=false&loop=false&delayms=60000" target="_blanck">TypeForm Demo</a>

Une fois le code d'intégration récupérer, il doit être collé là où l'on souhaite voir apparaitre le formulaire. On remarque que le code récupérér contient 2 parties : le bouton (dans une balise "a") et du JS (balise "script). Par souci de clartée nous avons séparré ces deux bouts de codes:

### Le bouton (l.219)
Pour que le bouton est le même aspect que les autres boutons du site, nous avons effacé l'attribut "style" et ajouté la classe "btn-pink".

```html
<a class="typeform-share button btn-pink" href="https://jonathanserafini.typeform.com/to/vUV9EH" data-mode="popup" target="_blank">Commender ici</a>
```

### Le JS (l.255-266)
Le javascript se met toujours à la fin avant </body>
```html
  <script>
    (function() {
      var qs,js,q,s,d=document, gi=d.getElementById, ce=d.createElement, gt=d.getElementsByTagName, id="typef_orm_share", b="https://embed.typeform.com/";
      if(!gi.call(d,id)){
        js=ce.call(d,"script");
        js.id=id;
        js.src=b+"embed.js";
        q=gt.call(d,"script")[0];
        q.parentNode.insertBefore(js,q)
      }
    })()
  </script>
```
## <a href="https://uikit.lewagon.com/" target="_blanck">Le wagon Ui components</a>

<a href="https://uikit.lewagon.com/" target="_blanck">Le wagon Ui components</a> est une bibliothèque de composents HTML/CSS mise à disposition par <a href="https://www.lewagon.com/" target="_blanck">Le wagon</a>. 

Il suffit de choisir un composant, de copier le HTML dans index.html puis le CSS dans style.css et de modifier le composant pour qu'il s'accorde avec le reste du site. Dans notre exemple nous allons remplacer le 1er cadre par une <a href="https://uikit.lewagon.com/documentation#banner" target="_blanck">bannière</a>

### Le HTML (l.66-74)
```html
  <div class="banner" style="background-image: linear-gradient(rgba(0,0,0,0.2),rgba(0,0,0,0.2)), url(images/banner.jpg);">
    <div class="container">
      <h1 class="color-green">Les Muffins de Grand Mère</h1>
      <h2 class="color-green">Fondants et croustillants</h2>
      <img src="images/muffin.jpg" alt="muffin" class="avatar">
      <br>
      <a href="https://www.marmiton.org/recettes/recette_muffins-tres-simples_166385.aspx" target="_blanck" class="btn-pink">En savoir plus</a>
    </div>
  </div>
```
### CSS (l.166-186)
```css
.banner {
  background-size: cover;
  background-position: center;
  padding: 150px 0;
}

.banner h1 {
  margin: 0;
  color: white;
  text-shadow: 1px 1px 3px rgba(0,0,0,0.2);
  font-size: 32px;
  font-weight: bold;
}

.banner p {
  font-size: 20px;
  color: white;
  opacity: .7;
  text-shadow: 1px 1px 3px rgba(0,0,0,0.2);
}
```

Nous avons légèrement changé le css et l'image de fond pour que cela corresponde plus a notre site.

