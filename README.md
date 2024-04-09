# Manual de usuario


*Equipo:* 11

*Integrantes:*

-Frida Pineda Alvarado

-Miguel Angel Reyes Martínez


En el presente trabajo se explicará el proceso que se llevo a cabo para esta pequeña parte de nuestro proyecto, el cual consiste en la resolución de ejercicios en el lenguaje Racket. Mostraremos los pasos que llevamos a cabo, desde la instalación y configuración del notebook, la solución de los ejercicios propuestos y descripción de la ejecución de cada uno de los problemas.


## Instalación y configuración del notebook ##

1. Para la instalación, ingresamos al sitio oficial de jupyter [enlace](https://jupyter.org/install). Copiamos y pegamos en la terminal el codigo que nos muestra en el apartado de Jupyter Notebook ***pip install notebook***.
![](https://github.com/frida348/Programaci-n-funcional/assets/112607095/b1125ae2-f643-4e98-8226-116ec77667ab)

2. Verificamos que se haya instalado corriendo el siguiente codigo en la terminal ***jupyter notebook***.
![](https://github.com/frida348/Programaci-n-funcional/assets/112607095/50349db6-5acf-4f84-9dcd-b9d3e34be776)

3. Por otra parte, nos aseguramos de tener Racket en nuestro sistema escribiendo lo siguiente en la terminal: ***racket --version***. En esta ocasión el comando "racket" no se encontraba en la variable de entorno PATH, así que lo agregamos manualmente.

4. Abrimos el "Panel de control" de Windows, buscamos "Sistema" y hacemos clic en "Editar variables de entorno del sistema".
![](https://github.com/frida348/Programaci-n-funcional/assets/112607095/baa63e67-9c94-4466-aed3-3b12b13df153)

6. En la ventana "Propiedades del sistema", hacemos clic en "Variables de entorno". En la sección "Variables del sistema", busca la variable llamada "Path" y selecciónala, luego haz clic en "Editar".
![](https://github.com/frida348/Programaci-n-funcional/assets/112607095/abc598f1-b0fa-4db3-a433-0522ac99bdd7)

7. Hacemos click en "Examinar" y seleccionamos la carpeta donde se encuentra instalado Racket. Aceptamos todo y guardamos.
![](https://github.com/frida348/Programaci-n-funcional/assets/112607095/2faf8229-6e97-4209-b3f3-41d7979ae31e)

8. Una vez que tenemos Racket, necesitamos instalar el paquete iracket, que proporciona el kernel de iRacket para Jupyter Notebook. Usamos el siguiente comando en la terminal: ***raco pkg install iracket***. Escribimos "Y" para instalar todas las dependencias.

9. Una vez hecho esto, buscamos dónde se encuentra el ejecutable iracket en nuestro sistema y agregamos esa ubicación a nuestra variable de entorno PATH (como hicimos con Racket previamente).
![](https://github.com/frida348/Programaci-n-funcional/assets/112607095/6a0552de-0451-4af7-9d81-8931fc03fbc4)

10. Ejecutamos el siguiente comando para registrar el kernel de IRacket con Jupyter: ***raco iracket install*** y procedemos a abrir nuestra notebook con el comando del paso 2: ***jupyter notebook***
![](https://github.com/frida348/Programaci-n-funcional/assets/112607095/d9579081-8ffb-475f-99c4-dd71e482d5a9)

11. Procedemos a crear un nuevo Proyecto
![](https://github.com/frida348/Programaci-n-funcional/assets/112607095/5f40d494-0051-48a7-a9be-031bac789879)

12. Creamos nuestras primeras notas :)
![](https://github.com/frida348/Programaci-n-funcional/assets/112607095/9edc3832-c38b-4c35-a51b-42038b621480)

## Descripción de cada problema ## 

