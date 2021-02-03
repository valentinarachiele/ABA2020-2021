#Raccolta di snippet utili per il templating su WordPress

- enqueue di un file (CSS, in questo caso) nel template
> nel file functions.php, dentro alla funzione function nomedeltema_scripts()

```wp_enqueue_style( 'simple-grid', get_template_directory_uri() . '/simple-grid.min.css', array(), _S_VERSION );```


- enqueue di un Google Font per cambiare il font del template e suo uso
> nel file functions.php, dentro alla funzione function nomedeltema_scripts()

```wp_enqueue_style( 'google-font', 'https://fonts.googleapis.com/css2?family=Hachi+Maru+Pop&display=swap', array(), _S_VERSION );```

- uso della griglia di simplegrid.io (il conto finale delle colonne dev'essere sempre 12)
> nel file corrispondente alla zona della pagina che si desidera modificare (ad esempio header.php e footer.php)

```
<div class="row"> <!-- questo è il contenitore generale della colonne -->
        <div class="col-5"> <!-- questa è una colonna che occupa 5/12 dello spazio -->
          <!-- qua ci va il contenuto desiderato (HTML e PHP) -->
        </div>
        <div class="col-7"> <!-- questa è una colonna che occupa 7/12 dello spazio -->
          <!-- qua ci va il contenuto desiderato (HTML e PHP) -->
        </div>
</div> <!-- chiudo .row -->
 ```
 
- togliere nel piede del sito tutti i riferimenti ad Altervista
> nel file style.css

```
.av-credit-link {
    visibility: hidden;
    display: none;
}
 ```
