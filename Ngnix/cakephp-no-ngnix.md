# Fazer o CakePHP funcionar no Ngnix com reescrita

Adicionar o conteúdo abaixo após o server_name

```bash
    # Feed to CakePHP for further processing!
    if (!-e $request_filename) {
        rewrite ^/(.+)$ /index.php?url=$1 last;
        break;
    }
```

Deve ficar algo do tipo:

```bash
	server_name localhost;

	# Not found this on disk?
    # Feed to CakePHP for further processing!
    if (!-e $request_filename) {
        rewrite ^/(.+)$ /index.php?url=$1 last;
        break;
    }
```