# Paso 6. Crea un pull request

<div align="center">
	<img src="https://ik.imagekit.io/gdgjaen/charlas/open-source-2021/tr:w-0.8/pull-request-hero_jgjXVemu3.png?updatedAt=1634136600060" />
</div>


## Creando un pull request (por GitHub)[^1]

### Desde la interfaz gráfica

1. Ve a tu repositorio en GitHub y verás un botón llamado `Pull request`.

   <div align="center">
   	<img src="https://ik.imagekit.io/gdgjaen/charlas/open-source-2021/tr:h-0.7/pull-request-boton_GD6udVZzWn.jpeg" />
   </div>

2. Escribe un título y una descripción para tu pull request.

   <div align="center">
   	<img src="https://ik.imagekit.io/gdgjaen/charlas/open-source-2021/tr:w-0.8/pullrequest-description_fY7qBmzgb.png" />
   </div>

3. <div align="center">
     </br>
   	<img src="https://ik.imagekit.io/gdgjaen/charlas/open-source-2021/tr:h-0.7/git-flowchart_2S6kARyK2Ir.png" />
   </br>
   </br>
   <i>El ciclo de vida del estado de tus archivos</i>
   </div>

### Desde la terminal

Es más eficiente y rápido hacerlo con GitHub CLI. 

GitHub CLI es una herramienta de línea de comandos con la que puedes hacer pull requests, crear issues y otras características de GitHub, para que puedas hacer todo en un solo lugar[^2].

#### Instalando GitHub CLI

1. [Instala](https://cli.github.com/) GitHub CLI. 

2. Autentícate.

   ```shell
   gh auth login
   ```

#### Pasos a seguir para hacer un pull request

1. Ubícate en la rama sobre la que quieres hacer el pull request. 

   ```shell
   git checkout NOMBRE_DE_LA_RAMA
   ```

2. Crea el pull request.

   ```shell
   gh pr create
   ```

   Sigue los pasos que te indican desde la terminal. 
   
   Este comando admite `flags`, para más información consulta la [documentación de GitHub CLI](https://cli.github.com/manual/gh_pr_create).

<div align="center" place-items="center">
  </br>
  <i>¡BRAVO! 🚀</i>
  <i>Acabas de hacer tu primer pull request</i>
</div>



[^1]: [Creating a pull request by GitHub](https://docs.github.com/en/github/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/creating-a-pull-request)
[^2]: [GitHub CLI](https://docs.github.com/en/github-cli/github-cli/about-github-cli)

