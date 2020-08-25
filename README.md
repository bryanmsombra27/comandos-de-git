## inicializar un repositorio local

```
git init
```

## añadir todos los archivos

```
git add .
```

## añadir todos los archivos cpn una extension de archivo expecifica

```
git add *.png
```

## excluir archivos que contengan una extension especifica del stage

```
git reset *.xml
```

## Viajes en el tiempo

- Para realizar viajes en el tiempo debemos colocar el siguiente comando y colocar un numero de version al que deseamos regresar para realizar alguuna modificacion a esa version

```
git reset  --soft  **nombre de la version a la que se quiere regresar en el tiempo**
```

## Viajes en el tiempo 2

- Si se utiliza este comando eliminara del repositorio todas aquellas versiones anteriores que le presedan a esta quiere decir que las de mas versiones seran eliminadas apartir del punto que se le indico

### Ejemplo:

```
 si se tiene 9 8 7 6 5

 - y se aplica el comando a  git reset  --hard 7

las versiones nuevas seran eliminadas  hasta el punto de referencia que es el 5 de tal forma que las versiones nos quedarian de la siguiente forma

   - 7  6 5

```

```
git reset  --hard  **nombre de la version a la que se quiere regresar en el tiempo**
```

## Guardar los cambios en los archivos (toma una captura del codigo como esta actualmente)

```
git commit -m "añade un mensaje  o una breve descripcion de los cambios realizados"
```

## checar status de los archivos

```
- git status
```

## añadir los cambios a un repositorio remoto

```
git push
```

## restaura todos los archivos del ultimo commit realizado

```
- git checkout -- .
```

## mostrar todos los commits realizados (ordenados por fechas del mas reciente hasta el mas antiguo)

```
git log
```

# Alias

## creando alias de manera global

- de esta forma configuramos un alias para que pueda ser reconocido en todos los repositorios con los que trabajemos dentro de las comillas debemos colocar el listado de comandos que correran una vez ejecutado el shorthand en este caso el comando lg

```
git config --global alias.lg "log  --oneline --decorate --all --graph"
```

```
git config --global alias.s "status  -s -b"
```

```
git config --global alias.tiempo"reset --hard"
```

## revisando la configuracion de nuestros alias

```
    git config --global -e //modo de escritura
```

```
    git config --global -l //modo de solo lectura
```

## Diferenciar entre cambios

- Podemos ver la diferencia entre los cambios del ultimo comit realizado y lo qu actualmente realizamos ( como parametro podemos indicarle que revise por la diferencia en los archivos que esten actualmente en el stage)

```
    git diff || git diff --staged
```

## Cambiar el mensaje a un commit

```
    git commit --amend -m "nuevo mensaje para el ultimo commit realizado"
```

## alternativa de escape cuando se utiliza el comando multilinea de git commit

- en caso de que olvidemos colocar el parametro -m entraremos al editor por defecto que contiene git para poder añadir un mensaje multilinea en caso de necesitarlo asique utilizando esa serie de pasos podemos salir del editor guardando los cambios
  ////////////////////////////////////////////////////////////////
  Prensa Escape. Esto debe asegurarse de que está en modo de comando
  escriba :wq
  Prensa Return
  /////////////////////////////////

/////////////////////////////////
