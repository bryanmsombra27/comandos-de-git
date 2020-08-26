## Comandos Repositorio Remoto

- Añadir un nuevo origen remoto

- por convencion el **nombre del repositorio** es llamado **origin**

```
git remote add nombre-del-repositorio  url-del-repositorio-remoto
```

## Revisar fuentes remotas

```
git remote -v
```

## añadir cambios a repositorio remoto

```
git push -u origin master
```

- Con este comando añadimos los cambios hacia el repositorio:
  **-u**: Nos permite indicarle que no se necesita especificar la rama la proxima vez que requiramos enviar los cambios al repositorio
  **origin**: El nombre del repositorio a la que se le enviaran los cambios
  **master**: el nombre de la rama en la que se almacenaran los cambios por default es master siempre que indica la rama principal

## Clonar un repositorio

```
git clone url-del-repositorio-remoto (parametro opcional para colocarle un nombre al repositorio por default se omite este parametro)
```
