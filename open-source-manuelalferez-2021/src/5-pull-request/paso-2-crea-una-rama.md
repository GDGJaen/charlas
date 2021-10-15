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

## Buenas prácticas 

El GitFlow Workflow es una metodología de trabajo basada en el división de las distintas etapas de producción de software en distintas ramas del repositorio [^2].

<div align="center">
	<img src="https://ik.imagekit.io/gdgjaen/charlas/open-source-2021/gitflow_gJcH9FOxg.svg" height="300px"/>
</div>

- `master`: En la rama máster se encuentran las *releases* estables de nuestro software. Esta es la rama que un usuario típico se descargará para usar nuestro software, por lo que todo lo que hay en esta rama debería ser funcional. Sin embargo, puede que las últimas mejoras introducidas en el software no estén disponibles todavía en esta rama.
- `develop`: En esta rama surge de la última release de `master`. En ella se van integrando todas las nuevas características hasta la siguiente release.

Y mucho más que puedes aprender en [Buenas prácticas al trabajar con Git por David Estevez](https://david-estevez.gitbooks.io/the-git-the-bad-and-the-ugly/content/es/buenas-practicas-al-trabajar-con-git.html).

Si te interesa saber más sobre el tema, te recomendamos leer [A successful Git branching model](https://nvie.com/posts/a-successful-git-branching-model/).

[^1]: [Explicación de Git branch: Cómo eliminar, mover, crear y renombrar una rama en Git por Obdulia Montiel](https://www.freecodecamp.org/espanol/news/explicacion-de-la-rama-de-gi-como-eliminar/#cambiar-de-rama)
[^2]: [Buenas prácticas al trabajar con Git por David Estevez](https://david-estevez.gitbooks.io/the-git-the-bad-and-the-ugly/content/es/buenas-practicas-al-trabajar-con-git.html)

