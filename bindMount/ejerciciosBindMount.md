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

1.  Crea un directorio en tu host y dentro crea un fichero `index.html.`

   ![Imagen de WhatsApp 2024-02-05 a las 12.39.04_eb0483ef](C:\Users\pablo\AppData\Local\Packages\5319275A.WhatsAppDesktop_cv1g1gvanyjgm\TempState\C15DA1F2B5E5ED6E6837A3802F0D1593\Imagen de WhatsApp 2024-02-05 a las 12.39.04_eb0483ef.jpg)

2. Crea un contenedor desde la imagen `php:7.4-apache` donde montes en el directorio
    `/var/www/html` el directorio que has creado por medio de bind mount .

  ![Imagen de WhatsApp 2024-02-05 a las 12.39.04_eb0483ef](C:\Users\pablo\AppData\Local\Packages\5319275A.WhatsAppDesktop_cv1g1gvanyjgm\TempState\C15DA1F2B5E5ED6E6837A3802F0D1593\Imagen de WhatsApp 2024-02-05 a las 12.39.04_eb0483ef.jpg)

3. Accede al contenedor desde el navegador para ver la información ofrecida por el fichero
    `index.html .`

  ![Imagen de WhatsApp 2024-02-05 a las 12.39.28_3bf1ca21](C:\Users\pablo\AppData\Local\Packages\5319275A.WhatsAppDesktop_cv1g1gvanyjgm\TempState\68053AF2923E00204C3CA7C6A3150CF7\Imagen de WhatsApp 2024-02-05 a las 12.39.28_3bf1ca21.jpg)

4. Modifica el contenido del fichero index.html en tu host y comprueba que al refrescar la
    página ofrecida por el contenedor, el contenido ha cambiado.

  ![Imagen de WhatsApp 2024-02-05 a las 12.41.18_68fabbe4](C:\Users\pablo\AppData\Local\Packages\5319275A.WhatsAppDesktop_cv1g1gvanyjgm\TempState\2DACE78F80BC92E6D7493423D729448E\Imagen de WhatsApp 2024-02-05 a las 12.41.18_68fabbe4.jpg)

![Imagen de WhatsApp 2024-02-05 a las 12.41.30_b4c96154](C:\Users\pablo\AppData\Local\Packages\5319275A.WhatsAppDesktop_cv1g1gvanyjgm\TempState\DF7F28AC89CA37BF1ABD2F6C184FE1CF\Imagen de WhatsApp 2024-02-05 a las 12.41.30_b4c96154.jpg)

5. Borra el contenedor.

    ![Imagen de WhatsApp 2024-02-05 a las 12.42.10_731472e5](C:\Users\pablo\AppData\Local\Packages\5319275A.WhatsAppDesktop_cv1g1gvanyjgm\TempState\96EA64F3A1AA2FD00C72FAACF0CB8AC9\Imagen de WhatsApp 2024-02-05 a las 12.42.10_731472e5.jpg)

6. Crea un nuevo contenedor y monta el mismo directorio como en el ejercicio anterior.

    ![Imagen de WhatsApp 2024-02-05 a las 12.47.38_aaab3727](C:\Users\pablo\AppData\Local\Packages\5319275A.WhatsAppDesktop_cv1g1gvanyjgm\TempState\DA8CE53CF0240070CE6C69C48CD588EE\Imagen de WhatsApp 2024-02-05 a las 12.47.38_aaab3727.jpg)

7. Accede al contenedor desde el navegador para ver la información ofrecida por el fichero
    `index.html` . ¿Se sigue viendo el mismo contenido?

    ![Imagen de WhatsApp 2024-02-05 a las 12.47.48_6566b62b](C:\Users\pablo\AppData\Local\Packages\5319275A.WhatsAppDesktop_cv1g1gvanyjgm\TempState\82489C9737CC245530C7A6EBEF3753EC\Imagen de WhatsApp 2024-02-05 a las 12.47.48_6566b62b.jpg)

  