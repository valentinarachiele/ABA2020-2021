#Raccolta di snippet utili per il templating su WordPress

1. enqueue di un file (CSS, in questo caso) nel template
wp_enqueue_style( 'simple-grid', get_template_directory_uri() . '/simple-grid.min.css', array(), _S_VERSION );
