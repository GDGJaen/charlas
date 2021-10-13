# Paso 3. Mantén tu fork actualizado

<div align="center">
  </br>
	<img src="https://ik.imagekit.io/gdgjaen/charlas/open-source-2021/fetch-git_dNAGsTgqxO.png" height="200px"/>
</div>




Estás contribuyendo a un proyecto de código abierto y notaste que tu fork no está sincronizado con el repositorio original. ¿Cómo puedes corregir eso?

## Sincronizando un fork (por GitHub) [^1]

### Desde la interfaz gráfica

Tan simple como hacer click en `Fetch upstream`: 

<div align="center">
  </br>
	<img src="https://ik.imagekit.io/gdgjaen/charlas/open-source-2021/sync-a-fork_5PsQ-nysuJ.png?updatedAt=1634119196564" height="300px"/>
</div>

### Desde la terminal [^2]

¿Sabías que tu fork es huérfano? Si listas el repositorio remoto configurado, solo verás tu fork como origen:

```shell
git remote -v
```

output:

```shell
origin  https://github.com/YOUR_USERNAME/YOUR_FORK.git (fetch)
origin  https://github.com/YOUR_USERNAME/YOUR_FORK.git (push)
```

Necesitamos configurar esta información para restaurar la relación familiar con el repositorio original al que le hicimos un fork:

1. Agregar un nuevo repositorio remoto conectado al proyecto del propietario

   <div align="center">
     </br>
   	<img src="https://ik.imagekit.io/gdgjaen/charlas/open-source-2021/updating-with-upstream_1PiPT6ys3.png" height="250px"/>
   </br>
   <i>Procesos que intervienen al sincronizar un fork</i>
   </div>

   

   ```shell
   git remote add upstream https://github.com/ORIGINAL_OWNER/ORIGINAL_REPOSITORY.git
   ```

2. ¡Salvaste a la familia! Ahora puedes ver el repositorio original y tu fork:

   ```shell
   git remote -v
   ```

   output:

   ```shell
   origin    https://github.com/YOUR_USERNAME/YOUR_FORK.git (fetch)
   origin    https://github.com/YOUR_USERNAME/YOUR_FORK.git (push)
   upstream  https://github.com/ORIGINAL_OWNER/ORIGINAL_REPOSITORY.git (fetch)
   upstream  https://github.com/ORIGINAL_OWNER/ORIGINAL_REPOSITORY.git (push)
   ```

3. Sincronizada tu fork. 

   1. Asegúrate que estás en la rama `master` de tu proyecto. 

      ```shell
      git checkout master
      ```

   2. Ahora, puedes traer los cambios del repositorio original a tu fork.

      ```shell
      git fetch upstream
      ```

      output:

      ```shell
      remote: Enumerating objects: 16, done.
      remote: Counting objects: 100% (16/16), done.
      remote: Compressing objects: 100% (7/7), done.
      remote: Total 7 (delta 5), reused 0 (delta 0), pack-reused 0
      Unpacking objects: 100% (7/7), 1.72 Kio | 160.00 Kio/s, done.
      From https://github.com/ORIGINAL_OWNER/ORIGINAL_REPOSITORY
         909ef5a..0b228a8  master     -> upstream/master
      ```

<div align="center" place-items="center">
  </br>
  <i>¡Hurra! 🥳</i>
  <i>Tu fork está sincronizado</i>
</div>

[^1]: [Syncing a fork by GitHub](https://docs.github.com/en/github/collaborating-with-pull-requests/working-with-forks/syncing-a-fork)
[^2]: [How to Sync Your Fork with the Original Git Repository by Johan Rin](https://www.freecodecamp.org/news/how-to-sync-your-fork-with-the-original-git-repository/)

