* HEALTHCHECK
  Es una instruccion que se agrega en el Dockerfile o en un docker run y define la manera de chequear la salud de un contenedor.  Los estados posibles son starting|healthy(0)|unhealthy(1)

* ONBUILD
  Es una instruccion que agrega un trigger a la imagen, para ejecutar posteriormente, cuando la imagen se usa como base para otro build.  Es como si se ejecutara seguido del "FROM".  
  Se puede ver con un docker inspect sobre la imagen.  Se pueden definir varios ONBUILD.

* VOLUME
  Es una instruccion para crear un punto de montaje que se comparte entre el host y los contenedores.
