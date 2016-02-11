# Apagar todos os arquivo de uma pasta recursivamente

Para apagar todos os arquivos dentro de uma pasta (tmp/ no exemplo), se tiver uma pasta dentro dela, apaga os arquivo dela também:


Exibindo os arquivos apagados:

```bash
find tmp/ -type f -exec rm -rv {} \;
```

Sem mostrar os arquivos apagados:

```bash
find tmp/ -type f -delete
```