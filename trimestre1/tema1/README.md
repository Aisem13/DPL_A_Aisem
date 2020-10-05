# Trabajando con Git y MarkDown

## Clonar Repositorio

para clonar un repositorio utilizaremos el siguiente comando:

![git clone](Images/Screenshot_1.png)

si el repositorio que queresmos clonar es privado nos pedirá el usuario y la contraseña, una vez que la pongamos  se nos clonará el repositorio en nuestro equipo,en el caso de que sea publico pasará directamente a clonar el repositorio a nuestro equipo.

## Crear archivo readme

Para crear nuestro archivo readme nos iremos a nuestra carpeta y luego ejecutamos el siguiente comando

![nano tarea1_1.md](Images/Screenshot_2.png)

## Hacer commit inicial

Lo primero que debemos hacer pasar nuestro archivos del working Directory al Staging Area, para ello utilizaremos el siguiente comando

![git add](Images/Screenshot_3.png)

el siguiente paso es hacer nuestro commit

![git commit](Images/Screenshot_4.png)

## Subir ficheros a repositorio remoto

Una vez hayamos echo el commit estaremos preparados para subir nustros archivos al repositorio remoto, solo tendremos que usar el siguiente comando

![git push](Images/Screenshot_5.png)

## Ignorar ficheros

Si tenemos algun fichero que queremos que git ignore solo tenemos que añadirlo al fichero .gitignore

![vim .gitignore](Images/Screenshot_6.png)

![añadir ficheros o carpetas](Images/Screenshot_7.png)

aquí podreis comprobar como git ignora tanto el fichero como el directorio que hemos puesto en .gitignore

![](Images/Screenshot_8.png)

## Añadir ficheros repositorio local

Si queremos añadir un fichero a nuestro repositorio local lo único que tenemos que hacer es utilizar el siguiente comando

![git add](Images/Screenshot_9.png)

## Crear tag

Para crear un tag solo tendreis que ejecutar el siguiente codigo

![git tag](Images/Screenshot_10.png)

ahora vamos a comprobar como se ha añadido el tag al commit  que hemos escogido

![git log](Images/Screenshot_11.png)

![](Images/Screenshot_12.png)

## Configuracion y Uso Github

### Poner foto perfil

para poner la foto de perfil no vamos a los ajustes y a la pestaña profile, una vez ahí clicamos en edit y elegimos la imagen que queremos poner

 ![](Images/Screenshot_13.png)
 
### doble factor de autenticación 

vamos a la pestaña account security y clicamos en el boton verde que nos pone enable Two-factor authentication

![](Images/Screenshot_14.png)
 
seguimos los pasos que nos dice y ya tendremos activada el doble factor de autenticación

![](Images/Screenshot_15.png)

### Seguir repositorio y dar estrellas

para seguir un repositorio solo tenemos que clicar en el ojo y elegir watch de este modo cada vez que se haga un cambio te lo notificará y para dar una estrella solo tendremos que clicar en la estrella

![](Images/Screenshot_16.png)

![](Images/Screenshot_17.png)

## Tabla github

| NOMBRE                            | GITHUB                         |
|-----------------------------------|--------------------------------|
| Francisco De Asís Domínguez Iceta | https://github.com/ciscoDIZ    |
| Enrique Granados Méndez           | https://github.com/enrique1999 |

# Trabajando con Git y MarkDown II

## Crear rama

Para crear una rama hemos de utilizar el siguiente código

![git branch](Images/Screenshot_18.png)

una vez creada la rama tenemos que posicionarnos en ella con él siguiente código

![git checkout](Images/Screenshot_19.png)

## Añadir fichero

una vez creado el fichero solo tendremos que usar el siguiente código para añadirlo

![git add](Images/Screenshot_20.png)

## Crear una rama remota

para crear una rama remota solo tendremos que usar este código 

![git push](Images/Screenshot_21.png)

## Merge directo

para hacer un merge primero hemos de situarnos en la rama master

![git checkout](Images/Screenshot_22.png)

Una vez situados en la rama master procederemos a hacer un merger de las dos ramas usando en siguiente código

![git merge](Images/Screenshot_23.png)

## Merge con conflicto

Vamos a crear en merge con conflicto para echo vamos a modificar en fichero 1.txt desde la ramas master y v0.2, en la rama master pondremos hola y en v0.2 pondremos adios en el mismo fichero

### rama master

modificando fichero 1.txt

![vim 1.txt](Images/Screenshot_24.png)

![](Images/Screenshot_44.png)

añadiendo el fichero y haciendo un comit

![git add](Images/Screenshot_25.png)

![git commit -m](Images/Screenshot_26.png)

### rama v0.2

modificando fichero 1.txt

![vim 1.txt](Images/Screenshot_27.png)

![](Images/Screenshot_45.png)

añadiendo el fichero y haciendo un comit

![git add](Images/Screenshot_28.png)

![git commit -m](Images/Screenshot_29.png)

una vez echo esto aremos el merge

![git commit -m](Images/Screenshot_30.png)


## Listar ramas

para listar ramas con merge usamos en siguiete código

![git branch --merge](Images/Screenshot_31.png)

![](Images/Screenshot_32.png)

y para las ramas sin merge este otro

![git branch --no-merge](Images/Screenshot_33.png)

![](Images/Screenshot_34.png)

## Arreglar conflico merge

Lo primero que tenemos que hacer es mirar las diferencias que hay, para ello haremos lo siguiente

![git diff](Images/Screenshot_35.png)

![](Images/Screenshot_36.png)

una vez vista la diferencia hay dos opciones o añadir la palabra adios en master o quitar esa palabra en v0.2, en este caso haremos la primera opción

![vim](Images/Screenshot_37.png)

![](Images/Screenshot_38.png)

luego lo añadimos y hacemos el commit

![git commit -m](Images/Screenshot_39.png)

y ya estamos listo para hacer el merge

![git merge](Images/Screenshot_40.png)

## Borrar la rama 

antes de borrar la rama vamos a crear un tag

![git tag](Images/Screenshot_41.png)

ahora procedemos a borra la rama

![git branch -d](Images/Screenshot_42.png)

## Listar cambios

para ver los cambios solo tendremos que usar el siguiente código

![git log --graph](Images/Screenshot_46.png)

y esto es lo que veremos

![git log --graph](Images/Screenshot_43.png)