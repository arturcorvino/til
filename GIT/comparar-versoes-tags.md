# Comparar versões por TAG OU COMMIT em projetos

Para ver os arquivos alterados e adicionados entre uma versão e outra, só executar o comando abaixo fazendo as substituições necessárias:

```bash
git diff --diff-filter=ACMRT --name-only <versao/commit anterior> <versao/commit nova>
```

Para ver os arquivos excluidos entre uma versão e outra, só executar o comando abaixo fazendo as substituições necessárias:

```bash
git diff --diff-filter=D --name-only <versao/commit anterior> <versao/commit nova>
```

Para copiar os arquivos alterados para uma pasta, só executar o comando abaixo fazendo as substituições necessárias:

```bash
cp -rfv $(git diff --diff-filter=ACMRT --name-only <versao/commit anterior> <versao/commit nova>) <diretorio destino> --parents
```

Para registrar os arquivos excluidos num documento.txt, só executar o comando abaixo fazendo as substituições necessárias:

```bash
git diff --diff-filter=D --name-only <versao/commit anterior> <versao/commit nova> > <diretorio destino>/deletados.txt
```

Para registrar os arquivos alterados num documento.txt, só executar o comando abaixo fazendo as substituições necessárias:

```bash
git diff --diff-filter=ACMRT --name-only <versao/commit anterior> <versao/commit nova> > <diretorio destino>/alterados.txt
```