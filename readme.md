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

Con estos pasos conseguimos subir un proyecto con git a un repositorio remoto.