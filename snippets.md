#Raccolta di snippet utili per il templating su WordPress

- enqueue di un file (CSS, in questo caso) nel template
> nel file functions.php, dentro alla funzione function nomedeltema_scripts()

```wp_enqueue_style( 'simple-grid', get_template_directory_uri() . '/simple-grid.min.css', array(), _S_VERSION );```


- enqueue di un Google Font per cambiare il font del template e suo uso
> nel file functions.php, dentro alla funzione function nomedeltema_scripts()

```wp_enqueue_style( 'google-font', 'https://fonts.googleapis.com/css2?family=Hachi+Maru+Pop&display=swap', array(), _S_VERSION );```
