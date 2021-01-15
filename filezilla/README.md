Configuración de despliegue de Filezilla en cluster GKE.

Para desplegar nuestro servicio de Filezilla, comenzaremos creando un despliegue en un archivo yaml.
Nuestro archivo, debe de ser de tipo Deployment.

En el apartado metadata, pondremos el nombre qué le vamos a dar a nuestro despliegue, a su vez, nos permitirá declarar una label (etiqueta).
Las etiquetas al igual que el nombre nos sirve para poder hacer referencia a nuestro despliegue.

En spec podemos declarar entre otros, el número de replicas qué haremos de cada despliegue, es decir, podemos elegir con cuantos contenedores comenzaremos en cada despliegue.

Otro punto importante es la selección de la imagen de los contenedores que vamos a desplegar. 
Nuestra idea es usar una imagen de Filezilla, en nuestro caso: https://hub.docker.com/r/jlesage/filezilla/
Es importante ver las instrucciones de cada contenedor para entender como usar la imagen.

Además de poner la imagen, pondremos los puertos qué usará nuestro contenedor internamente.
