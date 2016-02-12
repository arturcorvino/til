# Como criar atalhos para acesso ssh

Primeiro, é necessário gerar a chave SSH e adicionar ao servidor, pra não ser necessário solicitar a senha de acesso.

Depois execute no terminal:

```bash
$ vim ~/.ssh/config
```

E adicione um arquivo pra cada servidor, dessa forma:

```bash
Host alias
    HostName 127.0.0.1
    Port 43
    User usuarios
        IdentityFile ~/.ssh/id_rsa

Host <NOME>
    HostName <IP>
    Port <PORTA>
    User <USUARIO>
        IdentityFile ~/.ssh/id_rsa

```

Troque o alias pelo nome que será o servidor, exemplo: producao, teste.

```bash
$ ssh alias
```