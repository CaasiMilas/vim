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
# Atajos

| Comandos                | Que hacen                      | 
|-------------------------|--------------------------------|
|**hjkl**               	| Desplazamiento                 |
|**w e b**                | Movimiento entre palabras y esp|
|**[]**                   | Movimento por el codigo        |
|**{}**                   | Navegar entre bloques de codigo|
|**o**                  	| Escribir debajo de una linea   |
|**shift + o**            | Escribir arriba de una linea   |
|**ctrl + c**             | Salir de cualquier modo        |
|**ctrl + v**             | Modo de visual                 |
|**d**                  	| Borrar & char de mov. y desp.  |
|**dd**                  	| Borrar una linea               |
|**x**                  	| Borrar un caracter             |
|**X**                  	| Borrar un caracter anterior    |
|**$**                  	| Final de una linea             |
|**p**                    | Pegar el codigo                |
|**shift + p**          	| Pegar antes de                 |
|**i**                    | Escribir antes                 |
|**shift + i**           	| Escribir al inicio de una linea|
|**a**                    | Escribir despues               |
|**shift + a**            | Escribir al final de una linea |
|**r**                    | Reemplazar una letra           |
|**shift + r**            | Reemplazar un elemento         |
|**u**                    | Undo                           |
|**control + r**          | Reundo                         |
|**space + ,**            | copia una linea de bajo        |
|**space + n**            | Abre el buscador de archivos   |
|**%s/palabra1/palabra/g**| cambia palabra1 por la palabra |
|**yy y p**               | copia una linea                | 
|**yNUMEROy y p**         | copia multiples lineas         |

**Coc gestion para lenguajes**
| Lenguajes               | Que hacen                      |
|-------------------------|--------------------------------|
|**CocInstall**           | Instala los lenguajes          |
|**CocList**              | Listado de las opciones        |
|**Coclist>extensiones**  | Listado de los lenguajes       |
|**CocUpdate**            | Actualiza paquetes de lenguajes|

### Buscar coc vim para ver las opciones de los lenguajes
https://github.com/neoclide/coc.nvim/wiki/Language-servers
</br>
`Ver en CocList>extensiones si esta habilitado el lenguaje`
