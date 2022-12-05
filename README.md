# Los Estados de Git

## Espacio de Trabajo (Working Directory)
- Todo los archivos que podemos observar.

## Área de Trabajo (Staging Area)
- Son todos los archivos que está en estado `untracked` y pasan a `tracked` a través del comando `git add` 
## Repositorio (carpeta .git)
- Archivos llevados desde el Staging area -> repositorio GIT a través del comando `git commit`(archivo oculto)


## Comandos GIT: 


### GIT ADD
- Lleva archivos desde Wrongin Directory -> Staging Area.

        git add <name_archivo>


### GIT RESTORE
- Deshace los cambios, regresa al último commit anterior.

        git restore <Name_Archivo>



!["Estados de GIT"](./img/GitEstados.png)