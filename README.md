#  Taller Pull Request (PR)

Repo para hacer pruebas de PR en github. 

Y de paso obtener un lista de canciones para programar y de películas para ver 😉

Uso únicamente académico.

# Flujo de trabajo

## Solicitud de PR

1. Loguearse en GitHub

2. Ir a la [url del repo](https://github.com/0492-0616-0379-PI-DAM-DAW-ASIR/pull_request_workshop) y hacer un fork del repositorio 

3. Clonar fork en local

4. Crear una rama en el local para la nueva _feature_

    ```bash
    git checkout -b nueva_cancion
    ```

5. Añadir una (o más) nueva(s) canción(es) en el fichero _song4programming.md_

6. Hacer un _commit_ de la modificación

    ```bash
    git add song4programming.md
    git commit -m "feat: añadida nueva canción"
    ```
7. Subimos el _commit_ a nuestro repo 

    ```bash
    git push --set-upstream origin nueva_cancion
    ```

    > El uso de --set-upstream es debido a que la rama _nueva_cancion_ existe solo en local, y todavía no tiene ninguna relación con una rama en el servidor. _--set-upstream_ permite crearla en el remoto y vincularla. A partir de ese momento ya podremos usar simplemente _git push_.

    la salida del comando, entre otra información, nos indicará algo similar :
    
    ```bash
    remote: Create a pull request for 'nueva_cancion' on GitHub by visiting:
    remote:      https://github.com/GITHUB_USER/pull_request_workshop/pull/new/nueva_cancion
    ```

    Es decir, se nos indica que nos conectemos a nuestro _fork_ para poder solicitar un _PR_.

  8. Acceder a nuestro repo en GitHub y pulsar sobre _Compare & PR_

  9. Crear el PR

     * Indicar sobre quién y desde dónde se quiere hacer el PR. A la izquierda se indica el repo original y la derecha la rama de nuestro repo (el fork). En general viene configurado correctamente por defecto.

     * Indicar un título al PR. Por defecto viene asignado el mensaje del commit

     * Añadir una descripción. Es muy importante explicar con detalle que se ha hecho, que mejoras se añaden, qué errores se corrigen... 

     * Pulsamos en _Create Pull Request_

## Revisión

1. El revisor se loguea en GitHub

2. Una vez se accede al repo, en la barra superior aparecerán los PR pendientes.

3. El PR puede haber sido asignado a un revisor determinado o que alguien del equipo tenga una solictud para aceptar ser el revisor de ese PR. En este caso el revisor puede asignarse a si mismo u optar por solictar a otro(s) revisor(es) que se encarguen de ese PR.

4. Una vez está asignado, desde dentro del PR se puede acceder a la revisión.

5. Aprobar el PR, hacer un comentario o solicitar cambios para que pueda ser aprobada en un futuro.

6. Hacer la fusión con la rama principal. Para ello hay que elegir la estrategia de fusionado.

