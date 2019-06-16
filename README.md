# Jour 5

## <a href="https://mailchimp.com/" target="_blanck">MailChimp</a>

<a href="https://mailchimp.com/" target="_blanck">MailChimp</a> est un service en ligne qui permet de gérer des envoies de mails groupés. Il faut créer un "audience" (liste de mails destinataire de la future newsletter), un "template" (email type contenant la newletter) et enfin une "campagne" qui est l'action d'envoyer un template à une audience. 

Vous trouverez ici les imprim-écrans des différentes étapes à suivre pour intégrer un formulaire d'inscription à une audience (newsletter <a href="https://mailchimp.com/" target="_blanck">MailChimp</a>) :

<a href="https://docs.google.com/presentation/d/e/2PACX-1vRQPuy_5olP8j4p9P2KbDMsO_igLcq2mOWLcCuHNX7YECwDOi7e0WnyA1XM-8E1sDXk9dHxTcGE9E2g/pub?start=false&loop=false&delayms=3000" target="_blanck">Mailchimp demo</a>

Une fois le code d'intégration récupérer, il doit être collé là où l'on souhaite voir apparaitre le formulaire. On remarque que le code récupérér contient 3 parties : un lien vers une page de CSS (balise "link"), le formulaire et des du JS (balises "script). Par souci de clartée nous avons séparré ces trois bouts de codes:

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
