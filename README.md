# vim
# Instalamos vim

Para distribuciones de Arch
```
sudo pacman -S neovim
```

Para distribuciones de Debian
```
sudo apt-get install neovim
```

## Instalamos ranger

```
sudo pacman -S ranger
```

### Instalacion del vim plug

```
sh -c 'curl -fLo "${XDG_DATA_HOME:-$HOME/.local/share}"/nvim/site/autoload/plug.vim --create-dirs \
       https://raw.githubusercontent.com/junegunn/vim-plug/master/plug.vim'
```

### Algunas cosas necesarias

```
sudo pacman -S nodejs npm python python-pip ruby rubygems
```

### Descargando paquetes de neovim

```
pip install neovim
gem install neovim
sudo npm i -g neovim
```

### Dependencias 
``` 
sudo pacman -S xsel fzf ripgrep fd the_silver_searcher prettier 
yay -S universal-ctags-git 
``` 

Hacemos un `:PlugInstall` dentro de vim

# Atajos

| Comandos                | Que hacen                      | 
|-------------------------|--------------------------------|
|**hjkl**               	| Desplazamiento                 |
|**w e b**                | Movimiento entre palabras y esp|
|**[]**                   | Movimento por el codigo        |
|**{}**                   | Navegar entre bloques de codigo|
|**o**                  	| Escribir debajo de una linea   |
|**shift o**              | Escribir arriba de una linea   |
|**control + c**          | Salir de cualquier modo        |
|**control + v**          | Modo de visual                 |
|**d**                  	| Borrar & char de mov. y desp.  |
|**dd**                  	| Borrar una linea               |
|**x**                  	| Borrar un caracter             |
|**X**                  	| Borrar un caracter anterior    |
|**$**                  	| Final de una linea             |
|**p**                    | Pegar el codigo                |
|**shift + p**          	| Pegar antes de                 |
|**i**                    | Escribir                       |
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

**buscar coc vim para ver las opciones de los lenguajes**
</br>
`Ver en CocList>extensiones si esta habilitado el lenguaje`
