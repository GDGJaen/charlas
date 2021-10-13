# Paso 6. Crea un pull request

<div align="center">
	<img src="https://ik.imagekit.io/gdgjaen/charlas/open-source-2021/pull-request-hero_jgjXVemu3.png?updatedAt=1634136600060" height="200px"/>
</div>

## Creando un pull request (por GitHub)[^1]

### Desde la interfaz gráfica

1. Ve a tu repositorio en GitHub y verás un botón llamado `Pull request`.

   <div align="center">
   	<img src="https://ik.imagekit.io/gdgjaen/charlas/open-source-2021/pull-request-boton_GD6udVZzWn.jpeg" height="200px"/>
   </div>

2. Escribe un título y una descripción para tu pull request.

   <div align="center">
   	<img src="https://ik.imagekit.io/gdgjaen/charlas/open-source-2021/pullrequest-description_fY7qBmzgb.png" height="200px"/>
   </div>

3. Si tu pull request es aceptado recibirás un correo.

### Desde la terminal

Es más eficiente y rápido hacerlo cong GitHub CLI. 

GitHub CLI es una herramienta de línea de comandos con la que puedes hacer pull request, crear issues y otras características de GitHub desde terminal, para que pueda hacer todo tu trabajo en un solo lugar[^2].

#### Instalando GitHub CLI

1. [Instala](https://cli.github.com/) GitHub CLI. 

2. Autentícate.

   ```shell
   gh auth login
   ```

#### Pasos a seguir para hacer un pull request

1. Ubícate en la rama sobre la que quieres hacer el pull request. 

   ```shell
   git checkout BRANCH_NAME
   ```

2. Crea el pull request y sigue los pasos que te indica desde la terminal. 

   ```shell
   gh pr create
   ```

   Este comando admite flags, para más información consulta la [documentación de GitHub CLI](https://cli.github.com/manual/gh_pr_create).

<div align="center" place-items="center">
  </br>
  <i>¡BRAVO! 🚀</i>
  <i>Acabas de hacer tu primer pull request</i>
</div>



[^1]: [Creating a pull request by GitHub](https://docs.github.com/en/github/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/creating-a-pull-request)
[^2]: [GitHub CLI](https://docs.github.com/en/github-cli/github-cli/about-github-cli)

