# Pasos para subir un proyecto a Git
Partimos de la situación en que tenemos creado un proyecto git, que bien ha sido creado en local (git init),
o hemos obtenido de la nube (git clone). Realizamos las modificaciones necesarias, y llega el momento de añadir
esas modificaciones a nuestro repositorio en la nube:
1. Utilizando el comando ```git status``` verificamos que archivos del proyecto han sido modificados y aun no han sido actualizados en la nube.
2. Con el comando ```git add``` seleccionamos los archivos que queremos subir o actualizar, para añadirlos al
repositorio remoto. Podemos añadirlos uno por uno ```git add archivo1 archivo2 ...archivoN``` o todos los archivos modificados al mismo tiempo ```git add .```
3. Con el comando ```git commit -m "comentario"``` añadimos un titulo descriptivo para los cambios que hemos
realizado y que se van a incorporar al repositorio remoto.
4. Utilizando el comando ```git push``` incorporamos todos los cambios al repositorio remoto.

De esta forma conseguimos añadir nuestro proyecto local a un repositorio remoto.
# Reto 4 - Punto 3
No se puede realizar el push, da un error debido a que los cambios de nuestro repositorio local (rama actual)
están por detrás de los cambios del repositorio remoto. Esto se debe a que en el repositorio remoto existe la
carpeta "reto_2" con las imágenes, mientras que en el respositorio local, al utilizar .gitignore, procesa como
que esa carpeta no existe. Por ello, nos indica que antes de subir los cambios (push), obtengamos el estado del
repositorio remoto en local (pull).