# Desativar validação de modelo no controller

```php
<?php
	$this->Model->validate = array();
	
	if ($this->Model->save($save)) {

	}
 ?>
```

[fonte](http://devlearning.blogspot.com.br/2013/09/cakephp-using-plugin-component-in.html)
