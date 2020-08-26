## Trabajando con stash

- Con este comando podemos guardar el todo el trabajo que teniamos y dejarlo pendiente y luego volver a trabajar donde lo dejamos
  esto con el fin de no realizar un commit con trabajo que no ha sido probado o que puede causar que el sistema se quiebre

```
git stash
```

## listado de trabajo en progreso

-Con este comando podemos visualizar un listado en caso de tener algun trabajo pendiente que hayamos almacenado anteriormente

```
git stash list
```

## Obteniendo los cambios que almacenamos en el stash

- restaura y elimina la ultima version añadida del stash

```
git stash pop
```

## Obteniendo los cambios que almacenamos en el stash

- Restaura la ultima version añadida del stash

```
git stash apply
```

```
git stash apply
```

## Eliminando manualmente un stash almacenado

```
git stash drop nombre-del-stash || git stash drop ultima-entrada
```

## Eliminando manualmente un stash almacenado

```
git stash drop
```

- estos cambios seran guardados en el stash para poder trabajar con este texto despues
