# Paso 4. Crea un commit

<div align="center">
	<img src="https://ik.imagekit.io/gdgjaen/charlas/open-source-2021/tr:w-0.8/crea-un-commit_hbGzDMdb8B.png" />
</div>


Ya has creado esa magnífica feature. Toca registrarla en el historial de Git, realizando un commit. 

Los commits están en el corazón del uso de Git. Puedes pensar en un commit como una captura de tu proyecto, donde se crea una nueva versión de ese proyecto en el repositorio actual. Dos características importantes de los commits son:

- puedes recordar los cambios a los que se les hizo commits en una fecha posterior, o revertir el proyecto a esa versión
- si varios commits editan diferentes partes del proyecto, no se sobrescribirán entre sí aunque los autores de los commits no se conozcan entre sí. Este es uno de los beneficios de usar Git sobre una herramienta como Dropbox o Google Drive [^1]

> ¿Recuerdas cuando Antonio marcó con un marcador fluorescente los cambios que hizo a los apuntes de Susana y añadió un mensaje? 

## Pasos a seguir

<div align="center">
  </br>
	<img src="https://ik.imagekit.io/gdgjaen/charlas/open-source-2021/tr:h-0.7/git-flowchart_2S6kARyK2Ir.png" />
</br>
</br>
<i>El ciclo de vida del estado de tus archivos</i>
</div>



1. Antes de realizar el commit, indica a Git que quieres incluir actualizaciones en un archivo (o varios). Lo que se conoce como agregar el archivo a `staging`. 

   ```shell
   git add ARCHIVO1 ARCHIVO2
   ```

   Si quieres pasar a `staging` todos los archivos que han sido modificados:

   ```shell
   git add . 
   ```

2. Crea el commit.

   ```shell
   git commit -m "Mi mensaje"
   ```

   output: 

   ```shell
   [master 13vc6b2] Mi mensaje
    1 file changed, 1 insertion(+)
   ```

   La opción más utilizada con `git commit` es la opción `-m`. La `-m` significa mensaje. Cuando se llama a `git commit`, es necesario incluir un mensaje. El mensaje debe ser una breve descripción de los cambios que se han hecho. El mensaje debe estar al final del comando y debe estar envuelto entre comilla `" "`.



[^1]: [El Comando Git Commit Explicado por Juan Carrillo](https://www.freecodecamp.org/espanol/news/el-comando-git-commit-explicado/)

