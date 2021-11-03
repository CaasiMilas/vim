<p align="center">
  <a href="https://neovim.io/">
    <img alt="Neovim Log" src="https://upload.wikimedia.org/wikipedia/commons/4/4f/Neovim-logo.svg" height="130" />
  </a>
</p>
       
              
# Instalamos neovim en Linux

Para distribuciones de Arch
```
sudo pacman -S neovim
```

Para distribuciones de Debian
```
sudo apt-get install neovim
```

### Instalamos ranger

Para ditribuciones de Arch
```
sudo pacman -S ranger
```
Para distribuciones de Debian
```
sudo apt-get install ranger
```

### Instalacion de vim-plug via curl

```
sh -c 'curl -fLo "${XDG_DATA_HOME:-$HOME/.local/share}"/nvim/site/autoload/plug.vim --create-dirs \
       https://raw.githubusercontent.com/junegunn/vim-plug/master/plug.vim'
```

### Algunas cosas necesarias

Para distribuciones de Arch
```
sudo pacman -S nodejs npm python python-pip ruby rubygems
```
Para distribuciones de Debian
```
sudo apt-get install nodejs npm python python3-pip ruby rubygems
```

### Descargando paquetes de neovim

```
pip install neovim
gem install neovim
sudo npm i -g neovim
```

### Dependencias 

Para distribuciones de Arch
``` 
sudo pacman -S xsel fzf ripgrep fd the_silver_searcher prettier 
yay -S universal-ctags-git 
``` 
```
sudo apt-get install xsel fzf ripgrep silversearcher-ag
sudo npm install --save-dev --save-exact prettier
```
### Instalar universal-ctags-git via snap
https://snapcraft.io/universal-ctags

### Instalar plugins y extensiones envim
Abrimos neovim en la terminal y escribimos
```
:PlugInstall
```
```
:CocInstall coc-json coc-tsserver
```

## Coc Fallos en archivos
Si aparece una error de localizacion en los imports de coc, hacer lo siguiente:
```
:CocList folders
```
seleccionamos el folder ejemplo: `/home/user/python`

### Reiniciamos Coc
```
:CocRestart
```

# Atajos

| Comandos dentro de vim  | Que hacen                      | 
|-------------------------|--------------------------------|
|**:q**                   | Salir                          |
|**:qa!**                 | Forzar salida                  |
|**:w**                   | Guardar                        |
|**:wq**                  | Guardar y salir                |
|**:e**                   | Abrir archivo                  |

| Atajos de movimient
