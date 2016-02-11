# Como configurar o git para usar o Meld para corrigir conflitos

Instalar o meld:

```bash
$ sudo apt-get install meld
```

Configurar o git para usar o meld:

```bash
$ git config --global merge.tool meld
```

Usar o meld:

```bash
$ git mergetool
```