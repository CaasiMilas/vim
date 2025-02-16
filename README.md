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
sudo apt-get install nodejs npm python3-pip ruby rubygems
```

### Descargando paquetes de neovim

```
sudo pip install neovim
sudo gem install neovim
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

## Problemas de archivos con Coc
Si tenemos problemas de archivos con Coc ejecutar:
```
:CocList folders
```
**Seleccionamos el path en el que estamos trabajando ejemplo:** `/home/user/python`

Despues reiniciamos Coc
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

| Atajos de movimiento    | Que hacen                      | 
|-------------------------|--------------------------------|
|**hjkl**               	| Desplazamiento                 |
|**h**                    | Desplazamiento a la izquierda  |
|**j**                    | Desplazamiento hacia abajo     |
|**k**                    | Desplazamiento hacia arriba    |
|**l**                    | Desplazamiento a la derecha    |
|**w e b**                | Movimiento entre palabras y esp|
|**w**                    | Siguiente palabra              |
|**e**                    | Siguiente espacio              |
|**b**                    | Palabra anterior               |
|**[]**                   | Movimento por el codigo        |
|**{}**                   | Navegar entre bloques de codigo|
|**g + d**                | Definicion del mismo archivo   |
|**g + f**                | Definicion en otro archivo     |

| Atajos de edicion       | Que hacen                      |
|-------------------------|--------------------------------|
|**i**                    | Escribir                       |
|**I**                  	| Escribir al inicio de una linea|
|**a**                    | Escribir despues               |
|**A**                    | Escribir al final de una linea |
|**x**                  	| Borrar un caracter             |
|**X**                  	| Borrar un caracter anterior    |
|**o**                  	| Escribir debajo de una linea   |
|**O**                    | Escribir arriba de una linea   |
|**d**                  	| Borrar & char de mov. y desp.  |
|**D**                  	| Borrar una linea               |
|**d + w, e, b**          | Borrar con parametros          |
|**s**                    | Borrar caracter e insertar     |
|**S**                    | Borrar linea entera e insertar |
|**c + w, e, b**          | Borrar con parametros e insert |
|**C**                    | Borrar hacia el final e insert |
|**c + i + w**            | Reemplazar palabra             |
|**$**                  	| Final de una linea             |
|**0**                  	| Inicio de una linea            |
|**gg**                   | Ir al inicio del archivo       |
|**G**                    | Ir al final del archivo        |
|**1234 + G**             | Ir a la linea en especifico    |
|**/ + esc + n**          | Buscar despues del cursor      |
|**? + esc + n**          | Buscar antes del cursor        |
|**%**                    | Ir a la pareja de parentesis   |
|**p**                    | Pegar linea siguiente          |
|**P**                  	| Pegar linea anterior           |
|**r**                    | Reemplazar una letra           |
|**R**                    | Reemplazar un elemento         |
|**u**                    | Undo                           |
|**control + r**          | Reundo                         |
|**V**                    | Modo de visual                 |
|**control + c**          | Salir de cualquier modo        |
|**space + n**            | Abre el buscador de archivos   |
|**yy + p**               | copia una linea                | 
|**yNUMEROy + p**         | copia multiples lineas         |
|**:s/pal/palnew**        | Reemplazar con coincidencia    |
|**:s/pal/palnew/g**      | Reemplazar todas en la linea   |
|**:%s/pal/palnew/g**     | Reemplaza todas en el archivo  |
|! clear                  | Limpia instrucciones o cmds    |
## **Coc gestion para lenguajes**
| Lenguajes               | Que hacen                      |
|-------------------------|--------------------------------|
|**CocInstall**           | Instala los lenguajes          |
|**CocList**              | Listado de las opciones        |
|**Coclist>extensiones**  | Listado de los lenguajes       |
|**CocUpdate**            | Actualiza paquetes de lenguajes|
## **Map extensions vim**
| Explorer file           | Que hacen                      |
|-------------------------|--------------------------------|
|**:e + espacio + ctrl+d**| Abre un apartado de archivos   |
| NerdTree                | Que hacen                      |
## Keys
|Key                      | Action                         |
|-------------------------|--------------------------------|
|**espacio + n**          | Abre el explorador de archivos |
|**space + f**            | Fuzzy search                   |
|**space + /**            | Comenta la linea seleccionada  |
|**space + n**            | NerdTree                       |
|**space + p**            | Format con prettier            |
|**shift + k**            | Documentacion                  |



### Buscar coc vim para ver las opciones de los lenguajes
https://github.com/neoclide/coc.nvim/wiki/Language-servers
</br>
`Ver en CocList>extensiones si esta habilitado el lenguaje`
