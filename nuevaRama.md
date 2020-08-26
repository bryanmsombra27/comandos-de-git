# Esto sera parte de una nueva rama

## nueva rama

- creando una nueva rama

```
git branch  nombre-de-la-nueva-rama
```

## cambiando a la nueva rama

```
git checkout  nombre-de-la-nueva-rama
```

## uniendo ramas

```
git merge  nombre-de-la-nueva-rama
```

## eliminando una rama

```
git branch -d nombre-de-la-nueva-rama
```

## creando y cambiando a la nueva rama automaticamente

```
git checkout -b nombre-de-la-nueva
```

## creando etiquetas

- son referencias a un commit especifico (puede incluir el numero de version)

```
git tag nombre-de-la-etiqueta
```

## mostrando todas las etiquetas creadas

```
git tag
```

## eliminando una etiqueta en especifico

```
git tag -d nombre-de-la-etiqueta
```

## otra forma de crear las etiquetas

```
git tag -a v1.0.0 -m "nombre-de-la-etiqueta"
```
