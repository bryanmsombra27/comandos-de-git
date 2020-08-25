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

## creando alias de manera global

- de esta forma configuramos un alias para que pueda ser reconocido en todos los repositorios con los que trabajemos dentro de las comillas debemos colocar el listado de comandos que correran una vez ejecutado el shorthand en este caso el comando lg

```
git config --global alias.lg "log  --oneline --decorate --all --graph"
```

```
git config --global alias.s "status  -s -b"
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

## alternativa de escape cuando se utilzia el comando multilinea de git commit

////////////////////////////////////////////////////////////////
Prensa Escape. Esto debe asegurarse de que está en modo de comando
escriba :wq
Prensa Return
/////////////////////////////////
