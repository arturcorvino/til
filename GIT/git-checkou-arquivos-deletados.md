# Voltar os arquivos excluidos através do git checkout

Se por engano excluir alguns arquivos, antes de commitar, é possível voltar os mesmo através do comando:

```bash
git checkout $(git rev-list -n 1 HEAD -- "$file")^ -- "$file"
```