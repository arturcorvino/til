# Exibir todos os dias entre um intervalo de datas

Datas no formato pt_br (d/m/Y)

```php
//Star date
$dateStart 		= '20/04/2016';
$dateStart 		= implode('-', array_reverse(explode('/', substr($dateStart, 0, 10)))).substr($dateStart, 10);
$dateStart 		= new DateTime($dateStart);

//End date
$dateEnd 		= '25/04/2016';
$dateEnd 		= implode('-', array_reverse(explode('/', substr($dateEnd, 0, 10)))).substr($dateEnd, 10);
$dateEnd 		= new DateTime($dateEnd);

//Prints days according to the interval
$dateRange = array();
while($dateStart <= $dateEnd){
	$dateRange[] = $dateStart->format('d/m/Y');
	$dateStart = $dateStart->modify('+1day');
}

var_dump($dateRange);
```
Datas no formato padrão (Y-m-d)

```php
//Star date
$dateStart 		= '2016-04-20';
$dateStart 		= new DateTime($dateStart);

//End date
$dateEnd 		= '2016-04-25';
$dateEnd 		= new DateTime($dateEnd);

//Prints days according to the interval
$dateRange = array();
while($dateStart <= $dateEnd){
	$dateRange[] = $dateStart->format('Y-m-d');
	$dateStart = $dateStart->modify('+1day');
}

var_dump($dateRange);
```