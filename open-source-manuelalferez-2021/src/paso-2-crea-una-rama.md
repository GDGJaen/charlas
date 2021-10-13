# Paso 2. Crea una rama

<div align="center">
  </br>
	<img src="https://ik.imagekit.io/gdgjaen/charlas/open-source-2021/git-crear-rama_7oXZIjj-mI.png" height="300px"/>
</div>

Utilice una rama para aislar el trabajo de desarrollo sin afectar a otras ramas del repositorio. Cada repositorio tiene una rama predeterminada y puede tener varias otras ramas. 

Siempre crea una rama a partir de una rama existente. 

## Comandos importantes[^1]

Para ver las ramas en un repositorio Git, ejecuta el comando:

```shell
git branch
```

Para crear una nueva rama, ejecutar el comando:

```shell
git branch NOMBRE-NUEVA-RAMA
```

Para moverse a una rama existente, ejecuta el comando:

```shell
git checkout NOMBRE-RAMA
```

Hay un atajo para crear y moverte a la nueva rama al mismo tiempo.

```shell
git checkout -b NOMBRE-NUEVA-RAMA
```

Git no te permitirá eliminar una rama en la que te encuentres actualmente. Primero necesitas moverte a una rama diferente, y luego ejecutar el comando:

```shell
git branch -d RAMA-A-ELIMINAR
```

## ¿Tienes dificultades?

Tanto si es tu primera vez trabajando con Git como si tienes experiencia, es normal acudir a la documentación para consultar algún comando. 

Una lista de recursos útiles sobre Git: 

* [Guía de Git oficial en español](https://git-scm.com/book/es/v2). El libro completo de Git, escrito por Scott Chacon y Ben Straub. 
* [Guía de Git por GitHub (inglés)](https://guides.github.com/)
* [Guía de Git por Make it Real.](https://guias.makeitreal.camp/git) Una guía muy bien explicada y fácil de seguir. 
* [Tutorial de Git (YouTube).](https://www.youtube.com/playlist?list=PLTd5ehIj0goMCnj6V5NdzSIHBgrIXckGU) Si te va el contenido audiovisual, esta lista de reproducción te mostrará cómo utilizar Git, paso a paso, de forma clara.

[^1]: [Explicación de Git branch: Cómo eliminar, mover, crear y renombrar una rama en Git por Obdulia Montiel](https://www.freecodecamp.org/espanol/news/explicacion-de-la-rama-de-gi-como-eliminar/#cambiar-de-rama)

