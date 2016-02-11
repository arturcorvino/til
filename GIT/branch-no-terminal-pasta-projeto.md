# Exibir a branch no terminal quando tiver na pasta do projeto

Quando no Ubuntu, estiver numa pasta que é controlada a versão pelo git, para exibir a branch atual, basta abrir o arquivo ~/bashrc e substituir o valor da variavel:

De:

```bash
PS1='${debian_chroot:+($debian_chroot)}\[\033[01;32m\]\u@\h\[\033[00m\]:\[\033[01;34m\]\w\[\033[00m\] \$ '
```

Para 
```bash
PS1='\[\033[01;32m\]\u@\h\[\033[00m\]:\[\033[01;34m\]\w\[\033[00m\]\[\033[00m\]$(__git_ps1 " (%s)") \$ '
```



