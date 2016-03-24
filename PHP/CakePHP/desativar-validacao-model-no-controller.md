# Desativar validação de modelo no controller

```php
<?php
	$this->Model->validate = array();
	
	if ($this->Model->save($save)) {

	}
 ?>
```

[fonte](https://thedevelopersguide.wordpress.com/2013/07/31/disable-data-validation-in-controller-cakephp/)
