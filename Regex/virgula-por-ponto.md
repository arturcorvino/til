# Subistituir virgula por ponto entre números

## Problema:

Trocar as virgulas por ponto, somente o que estiver entre números:

```sql
INSERT INTO TESTE (NOME, CIDADE, VALOR) VALUES ('Bruno','Simonsen','0,5');
INSERT INTO TESTE (NOME, CIDADE, VALOR) VALUES ('Pedro','Votuporanga','20,15');
INSERT INTO TESTE (NOME, CIDADE, VALOR) VALUES ('Joao','Rio de Janeiro','220,5');
INSERT INTO TESTE (NOME, CIDADE, VALOR) VALUES ('Maria','Bahia','0,9');
```

## Solução:

### REGEX: 

ctrl + h no sublime

DE:

``` ([0-9]),([0-9]) ```

PARA:

``` $1.$2 ```

```sql
INSERT INTO TESTE (NOME, CIDADE, VALOR) VALUES ('Bruno','Simonsen','0.5');
INSERT INTO TESTE (NOME, CIDADE, VALOR) VALUES ('Pedro','Votuporanga','20.15');
INSERT INTO TESTE (NOME, CIDADE, VALOR) VALUES ('Joao','Rio de Janeiro','220.5');
INSERT INTO TESTE (NOME, CIDADE, VALOR) VALUES ('Maria','Bahia','0.9');
```