# Paso 5. Push

Tenemos nuestro commit, toca subir los commits desde tu rama local en tu repositorio Git local al repositorio remoto.

> Antonio escaneando los apuntes para subirlos a su nube. 

Basta con el siguiente comando: 

```shell
git push REPOSITORY_NAME BRANCH-NAME
```

Donde `REPOSITORY_NAME` puedes encontrarlo con:

```shell
git remote -v
origin    https://github.com/YOUR_USERNAME/YOUR_FORK.git (fetch)
origin    https://github.com/YOUR_USERNAME/YOUR_FORK.git (push)
upstream  https://github.com/ORIGINAL_OWNER/ORIGINAL_REPOSITORY.git (fetch)
upstream  https://github.com/ORIGINAL_OWNER/ORIGINAL_REPOSITORY.git (push)
```

En este caso,`origin` es el nombre de nuestro fork, ya que es el que está asocidado a nuestro fork: 

<div>
  <code>origin	https://github.com/<b>YOUR_USERNAME/YOUR_FORK.git</b></code>
</div>

## ¿Quieres más?

La [guía de GitHub](https://github.com/git-guides/git-push) acerca `push` es lo que buscas. 

