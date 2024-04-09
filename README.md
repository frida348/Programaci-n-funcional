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

1. **Función combinatorio(n, k)**: Esta función calcula el número combinatorio C(n, k) utilizando una definición recursiva. El número combinatorio C(n, k) es el número de formas de seleccionar k elementos de un conjunto de n elementos. La función retorna 0 si n es menor que k, 1 si k es 0 o n es igual a k, y en otros casos, llama a sí misma recursivamente con los argumentos (n-1, k-1) y (n-1, k), y suma los resultados.

2. **Función mcd(a, b)**: Esta función calcula el Máximo Común Divisor (MCD) de dos enteros a y b utilizando la propiedad de que MCD(a, b) = MCD(a, b-a). La función imprime a si a es igual a b, llama a sí misma con los argumentos (a, b-a) si a es menor que b, y con los argumentos (b, a) si a es mayor que b.

3. **Función primos**: La función primo verifica si un número n es primo, iterando desde 2 hasta la raíz cuadrada de n para buscar un divisor. Si encuentra alguno, retorna #f; de lo contrario, retorna #t. La función primos genera una lista de números primos entre inicio y fin. Si inicio es mayor que fin, retorna una lista vacía. Para cada número en el rango, si es primo, lo agrega a la lista y avanza al siguiente número; de lo contrario, solo avanza al siguiente número. Al final, retorna la lista de primos encontrados.

4. **Función busqueda(lista, n)**: Esta función busca un elemento n en una lista. Retorna `#t` (verdadero) si n es un miembro de la lista, y `#f` (falso) si n no es un miembro de la lista.

5. **Función invertir(lista)**: Esta función invierte una lista utilizando una función auxiliar llamada acumulador. La función acumulador toma una lista y una lista de resultados como argumentos, y se llama a sí misma recursivamente con el resto de la lista y el resultado concatenado con el primer elemento de la lista.

6. **Función eliminar(lista, n)**: Esta función elimina un elemento n de una lista utilizando una función auxiliar llamada eliminador. La función eliminador recorre la lista recursivamente, omite el elemento n si lo encuentra, y conserva el elemento si no es n.

7. **Función palindromo(n)**: Esta función verifica si un número entero n es un palíndromo. Convierte el número n a una cadena de caracteres, calcula la longitud de la cadena, y luego verifica si el primer y el último carácter de la cadena son iguales. Si son iguales, llama a sí misma recursivamente en el resto de la cadena.

8. **Función SumaDigitos(n)**: Esta función encuentra la suma de los dígitos de un número entero n. Utiliza la recursión para dividir n por 10 hasta que n sea un número de un solo dígito. En cada paso de la recursión, calcula el residuo de n dividido por 10 (el último dígito de n) y lo suma al resultado de la llamada recursiva a SumaDigitos con n dividido entre 10 (n con su último dígito eliminado).

9. **Función Binario(n)**: Esta función convierte un número entero n a binario. Utiliza la recursión para dividir n por 2 hasta que n sea menor que 2. En cada paso de la recursión, calcula el residuo de n dividido por 2 (el último dígito binario de n) y lo agrega a la lista de dígitos binarios.

10. **Función para calcular PI**:
