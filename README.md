# Los Estados de Git

## Espacio de Trabajo (Working Directory)
- Todo los archivos que podemos observar.

## Área de Trabajo (Staging Area)
- Son todos los archivos que está en estado `untracked` y pasan a `tracked` a través del comando `git add` 
## Repositorio (carpeta .git)
- Archivos llevados desde el Staging area -> repositorio GIT a través del comando `git commit`(archivo oculto)



!["Estados de GIT"](./img/GitEstados.png)


## Comandos GIT: 


### GIT ADD
- Lleva archivos desde Working Directory -> Staging Area.

        git add <name_archivo>


### GIT RESTORE
- Deshace todos los cambios en el working directory.

        git restore <name_archivo>


### GIT RESTORE --STADGE
- regresa el archivo de Staging area -> working directory

        git restore --staged <archivo>


### GIT RESTORE --STAGED --WORKTREE 
- regresa el archivo de staging area a working directory para luego eliminar todo los cambios del archivo.

        git restore --staged --worktree <archivo>


### GIT RESTORE .
- deshace todos los cambios hechos en el Working directory de todos los archivos.

        git restore .
        
esto se elimina
### GIT COMMIT -AM
- Todos los archivos Modificados van a pasar a Stagin Area -> Directorio Git en un solo paso con el siguiente comando

        git commit -am "message"
 
### GIT COMMIT -M "CABECERA DEL COMMIT" -M "CUERPO DEL COMMIT" 
- Forma de excribir buenos mensaje de Commits

        git commit -m "" -m ""

### GIT CHECKOUT -- <archivo>
- Trae el commit de main (HEAD) y lo aplica por encima de los cambios, con esto lo deja como estaba al principio.

        git checkout -- <archivo>
        git checkout <archivo>

### GIT CHECKOUT -F
- Trae el commit anterior proximo de la cabecera (HEAD) y lo aplica por encima de los cambios hechos en working directory, todo esto para todos los archivos.

        git checkout -f

### GIT LOG 
- Comando que muestra todos los commits en el historial del repositorio. Por defecto, muestra los datos de cada commit.

        git log

### GIT LOG --ONELINE
- Muestra los commits en el historial de  `manera resumida`.

        git log --oneline

### GIT STATUS
- Muestra el estado del directorio de trabajo y del àrea del entorno de trabajo.

        git status

### DOCUMENTACION DEL PROYECTO
- creación de repositorio.
- trabajos colaborativos.
- etc.