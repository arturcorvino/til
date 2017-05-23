# Install ZSH

```bash
sudo apt-get install zsh
```
> Restart your terminal. Choose option 2 for Z Shell configuration.  
> Don't forget to migrate your previous configurations (RVM, Rbenv...) from ```.bashrc``` to ```.zshrc```

## Install Oh My ZSH

```bash
cd
sh -c "$(curl -fsSL https://raw.github.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"
```

## Setup missing fonts (powerline)

### Install powerline font
```bash
cd
wget https://github.com/powerline/powerline/raw/develop/font/PowerlineSymbols.otf
wget https://github.com/powerline/powerline/raw/develop/font/10-powerline-symbols.conf
mv PowerlineSymbols.otf ~/.fonts/
mkdir -p .config/fontconfig/conf.d #if directory doesn't exists
```

### Clean fonts cache
```bash
fc-cache -vf ~/.fonts/
```

### Move config file
```bash
mv 10-powerline-symbols.conf ~/.config/fontconfig/conf.d/
```

## Configure ZSH

```bash
vim ~/.zshrc
```

### Theme
Change [ZSH_THEME="robbyrussell"] to [ZSH_THEME="agnoster"]
```bash
ZSH_THEME="agnoster"
```

## Guake

Preferences -> Sheel -> Select "/bin/zsh"

[font1](https://gist.github.com/renshuki/3cf3de6e7f00fa7e744a)
[font2](https://bosnadev.com/2015/02/26/awesome-looking-terminal-with-oh-my-zsh/)