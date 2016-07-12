# Para as execuções do crond do CentOS / RHEL pegar a data UTC


```bash
crontab -e
```

Adicionar no começo do arquivo:

```bash
TZ=America/Sao_Paulo
```

Restartar servicos necessários:

```bash
sudo service rsyslog restart

sudo service crond restart

```

[fonte](http://serverfault.com/questions/314697/timezone-for-cron-jobs)