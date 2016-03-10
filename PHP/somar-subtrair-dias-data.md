# Somar ou Subtrair dias de uma data

## Somar 

10 dias a partir de hoje

```php
echo date('d/m/Y', strtotime("+10 days"));
```

10 dias a partir de uma data

```php
echo date('d/m/Y', strtotime("+10 days",strtotime('20-07-2011')));
```

## Subtrair

10 dias a partir de hoje

```php
echo date('d/m/Y', strtotime("-10 days"));
```

10 dias a partir de uma data

```php
echo date('d/m/Y', strtotime("-10 days",strtotime('20-07-2011')));
```