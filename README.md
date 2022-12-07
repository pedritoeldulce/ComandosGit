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

### GIT COMMIT -AM
- Todos los archivos Modificados van a pasar a Stagin Area -> Directorio Git en un solo paso con el siguiente comando

        git commit -am "message"
 

### GIT CHECKOUT -- <archivo>
- Trae el commit de main (HEAD) y lo aplica por encima de los cambios, con esto lo deja como estaba al principio.

        git checkout -- <archivo>

### DOCUMENTACION DEL PROYECTO
- creación de repositorio.
- trabajos colaborativos.
- etc.