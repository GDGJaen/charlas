# Introducción a Git

La manera en la que Git trabaja puede ser intimidante al principio. Con una metáfora entenderemos mejor qué es eso de los pull request, repositorio local, repositorio en la nube, push, pull, etc. 

Imaginemos dos estudiantes, Susana y Antonio. Susana vive en Canada y Antonio en España. 

Susana hace muy buenos apuntes de matemáticas. La manera en la que ella trabaja es la siguiente: 

1. Escribe las notas a mano
2. Después las escanea y las pasa a su ordenador, porque no quiere perder su valiosos apuntes 

<div align="center">
	<img src="https://ik.imagekit.io/gdgjaen/charlas/open-source-2021/git-metafora_vaJtliQGf.png" height="300px"/>
</div>

Antonio le pide a Susana la copia de su ordenador y ella acepta encantada. 

<div align="center">
	<img src="https://ik.imagekit.io/gdgjaen/charlas/open-source-2021/metafor-fork_15qC4Vye_.png" height="150px"/>
</div>

Ahora tanto Susana como Antonio tiene una copia exacta de los apuntes de matemáticas.

> En Git, a esto se le conoce como hacer un `fork` de un proyecto. 

Antonio le pasa como a Susana, le gusta trabajar en su cuaderno físico. Sabemos que Antonio no es tonto, no estaba dispuesto a pasar todos los apuntes a mano, por ello fue a la copistería de Jacinta e imprimió los apuntes de Susana. 

> En Git, esto se le conoce como hacer un `pull` de nuestro repositorio en la nube a nuestro repositorio local. 

Pasados unos días, Antonio descubre que había un cálculo mal hecho en los apuntes de Susana y se dispone a corregirlo en su cuaderno. 

Sin embargo, Susana ha sido muy buena pasándole los apuntes a Antonio. Antonio quiere agradecerle su gesto notificicándole la errata que encontró. 

¡Houston, tenemos un problema! Antonio lo ha corregido en su cuaderno, pero no puede enviarle su cuaderno a Susana. Espera, ¡sí puede! de la misma forma que hizo Susana. 

Antonio señala con un marcador fluorescente el error y más abajo añade la corrección. 

> En Git, esto se le conocerá como hacer un `commit`, es decir, registrar los cambios que se le han hecho al documento original. Los commits, como ya veremos, llevan asociados mensajes descriptivos. 

<div align="center">
	<img src="https://ik.imagekit.io/gdgjaen/charlas/open-source-2021/commit-metafora_e0ECl7ZGr.png" height="300px"/>
</div>

Ahora sí, Antonio puede escanear los apuntes, subirlos a su nube y notificar a Susana de los cambios realizados. 

Más adelante, Susana revisará la aportación de Antonio para: 

* si Antonio no tiene razón, descartar actualizar sus apuntes 
* si por el contrario, Antonio tiene razón, Susana corregirá sus apuntes para no sacar un cerapio

> En Git, esto se le conoce como hacer un `pull request`, es decir, notificar al creador original de los apuntes sobre una posible mejora. 

## Conoce más sobre Git

Tanto si es tu primera vez trabajando con Git como si tienes experiencia, es normal acudir a la documentación para consultar algún comando. 

Una lista de recursos útiles: 

* [Guía de Git oficial en español](https://git-scm.com/book/es/v2). El libro completo de Git, escrito por Scott Chacon y Ben Straub. 
* [Guía de Git por GitHub (inglés)](https://guides.github.com/)
* [Guía de Git por Make it Real](https://guias.makeitreal.camp/git)  
* [Tutorial de Git (YouTube).](https://www.youtube.com/playlist?list=PLTd5ehIj0goMCnj6V5NdzSIHBgrIXckGU) Si te va el contenido audiovisual, esta es tu lista de reproducción. 
