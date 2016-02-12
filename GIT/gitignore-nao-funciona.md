# .gitignore não funciona? Como resolver?

No inicio de um projeto eu criei um novo repositório git e fiz vários commits, o que aconteceu foi que lá na frente eu percebi que devia ter ignorado alguns arquivos que não são necessários ser versionados, adicionei o .gitignore ao projeto e pra minha surpresa ele não quis funcionar, pois eu já havia comitado esses arquivos, tive uma baita dor de cabeça para descobrir o motivo, e como resolver, mas descobri,a solução é a seguinte:

```bash
git rm -r --cached .
```