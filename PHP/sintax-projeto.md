# Verificar sintax de todos os arquivos do projeto

Para verificar a sintax dos arquivos com a extensão .php monitorados pelo git, execute o comando no terminal:

```bash
git ls-tree -r HEAD --name-only |grep -E \(\.php\)\$ |xargs -L 1 php -l
```

Para verificar a sintax dos arquivos com a extensão .php e .ctp monitorados pelo git, execute o comando no terminal:

```bash
git ls-tree -r HEAD --name-only |grep -E \(\.php\|\.ctp\)\$ |xargs -L 1 php -l
```
