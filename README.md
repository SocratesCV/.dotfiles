# Todos los archivos de configurción 
Archivos de configuración de linux, tendré que ir actualizando, añadiendo y modificando poco a poco. 
Pero reuniéndolos aquí, puedo tener en todos los ordenadores la misma configuración de una manera sencilla.

## Cómo utilizarlo
Dentro del directorio personal, utilizar el comando:
`git clone https://github.com/SocratesCV/.dotfiles.git`


Con esto se creará un directorio .dotfiles y dentro todos los archivos de configuración.
''' mkdir ~/.dotfiles/i3/.config/i3 '''
Ahora solo queda remplazar y enlaza los archivos originales.
Creamos los archivos vacío dentro de su ubicación:
< touch config>
Después cremos los enlaces simbólicos con la aplicación stow:
` stow --adopt -nv i3`  
La opción -n es para ver si hay algún error, hace una simulación de los enlaces simbólicos, si todo está bien se puede quitar esa opción y ya se ejecuta.
` stow --adopt -v i3` 
Subimos todo a github
`git add . ` Para añadir todos los archivos modificados.
`git commit -m "Mensaje explicativo"` Comentamos la modificación.
`git push origin master`  Subimos las modificaciones a la rama principal.

Para recuperar los archivos en otro equipo:
`git clone  https://github.com/SocratesCV/.dotfiles.git`
`cd ~/.dotfiles`
`stow -v i3` Crea los enlaces simbólicos necesarios.

## Alacritty
### Descripción:
Aplicación de terminal
### .alacritty.yml
Practicamente está la configuración por defecto, iré cambiando y modificando la configuración según vaya haciendo falta.

## Bashrc
### Descripción:

## .bashrc
Tengo que añadir mi configuración y las variables. De momento está por defecto.

## Vim
### Descripción 
  Archivo de configuración de vim, 
    Si da el error 309 por no reconocer alguna librería de python se puede solucionar intalando el paquete:
`sudo apt install vim-nox-py2`  
### .vimrc
Este archivo ha sido creado automaticamente por la distribución archo linux.



