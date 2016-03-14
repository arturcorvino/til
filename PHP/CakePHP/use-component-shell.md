# Usar componente em shell

```php
<?php
	App::uses('ComponentCollection', 'Controller');
	App::uses('MyPluginClassComponent', 'MyPlugin.Controller/Component');

	class TestShell extends AppShell {

		public function main() {
			$collection = new ComponentCollection();
			$this->MyPluginClass = new MyPluginClassComponent($collection);
			$this->MyPluginClass->helloworld();
		}

	}
 ?>
```

[fonte](http://devlearning.blogspot.com.br/2013/09/cakephp-using-plugin-component-in.html)
