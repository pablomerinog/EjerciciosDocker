### Ejercicios Volúmenes

1. Crea un volumen docker que se llame miweb .

   ![image-20240205114819678](./../../../../../Escritorio/DESPLIEGUE/typora-user-images/image-20240205114819678.png)

2. Crea un contenedor desde la imagen php:7.4-apache donde montes en el directorio
    /var/www/html (que sabemos que es el DocumentRoot del servidor que nos ofrece esa
    imagen) el volumen docker que has creado.

  ![image-20240205114850251](./../../../../../Escritorio/DESPLIEGUE/typora-user-images/image-20240205114850251.png)

3. Utiliza el comando docker cp para copiar un fichero index.html en el directorio
    /var/www/html .
    
    Utilicé el comando docker exec en vez de docker cp por que me daba problemas.
    
    ![image-20240205114952006](./../../../../../Escritorio/DESPLIEGUE/typora-user-images/image-20240205114952006.png)

  

4. Accede al contenedor desde el navegador para ver la información ofrecida por el fichero
    index.html .

  ![image-20240205115012643](./../../../../../Escritorio/DESPLIEGUE/typora-user-images/image-20240205115012643.png)

5. Borra el contenedor.

   ![image-20240205115151636](./../../../../../Escritorio/DESPLIEGUE/typora-user-images/image-20240205115151636.png)

6. Crea un nuevo contenedor y monta el mismo volumen como en el ejercicio anterior.

   ![image-20240205115844088](./../../../../../Escritorio/DESPLIEGUE/typora-user-images/image-20240205115844088.png)

7. Accede al contenedor desde el navegador para ver la información ofrecida por el fichero
    index.html . ¿Seguía existiendo ese fichero?

​	![image-20240205115911613](./../../../../../Escritorio/DESPLIEGUE/typora-user-images/image-20240205115911613.png)

### Ejercicios Bind Mount

1.  Crea un directorio en tu host y dentro crea un fichero index.html.

   

2. Crea un contenedor desde la imagen php:7.4-apache donde montes en el directorio
    /var/www/html el directorio que has creado por medio de bind mount .

  

3. Accede al contenedor desde el navegador para ver la información ofrecida por el fichero
    index.html .

  

4. Modifica el contenido del fichero index.html en tu host y comprueba que al refrescar la
    página ofrecida por el contenedor, el contenido ha cambiado.

  

5. Borra el contenedor.

   

6. Crea un nuevo contenedor y monta el mismo directorio como en el ejercicio anterior.

   

7. Accede al contenedor desde el navegador para ver la información ofrecida por el fichero
    index.html . ¿Se sigue viendo el mismo contenido?

  