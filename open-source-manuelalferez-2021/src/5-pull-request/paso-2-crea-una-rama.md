# Paso 2. Crea una rama

<div align="center">
  </br>
	<img src="https://ik.imagekit.io/gdgjaen/charlas/open-source-2021/git-crear-rama_7oXZIjj-mI.png" height="300px"/>
</div>

Utilice una rama para aislar el trabajo de desarrollo sin afectar a otras ramas del repositorio. Cada repositorio tiene una rama predeterminada y puede tener varias otras ramas. 

## Comandos importantes[^1]

Para ver las ramas existentes, ejecuta el comando:

```shell
git branch
```

Para crear una nueva rama, ejecutar el comando:

```shell
git branch NOMBRE_NUEVA_RAMA
```

Para moverse a una rama existente, ejecuta el comando:

```shell
git checkout NOMBRE_RAMA
```

Hay un atajo para crear y moverte a la nueva rama al mismo tiempo.

```shell
git checkout -b NOMBRE_NUEVA_RAMA
```

Git no te permitirá eliminar una rama en la que te encuentres actualmente. Primero necesitas moverte a una rama diferente, y luego ejecutar el comando:

```shell
git branch -d RAMA_A_ELIMINAR
```

[^1]: [Explicación de Git branch: Cómo eliminar, mover, crear y renombrar una rama en Git por Obdulia Montiel](https://www.freecodecamp.org/espanol/news/explicacion-de-la-rama-de-gi-como-eliminar/#cambiar-de-rama)

