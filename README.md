# PRIMER PARCIAL DEL CURSO SISTEMAS OPERACIONALES


**PUNTO 1**

*Seleccione 5 retos de la página https://cmdchallenge.com y presente la solución a cada uno de ellos a través de un ejemplo práctico en 
CentOS7. Presente capturas de pantalla relevantes como evidencias de lo realizado.*

•	*find_a_string_in_a_file*

  Se imprimen las líneas que contienen “de”. Para ello, creo un archivo llamado prueba.txt
  ![1a](https://cloud.githubusercontent.com/assets/17281733/23804104/c1ad7cea-0586-11e7-951e-a8ff4c20a284.png)

  Uso comando “grep”
  
  ![1b](https://cloud.githubusercontent.com/assets/17281733/23804141/e0750c10-0586-11e7-8f04-7ce57e3af38b.png)
 
 
•	*search_for_files_containing_string*
  
  Se tienen 3 archivos: prueba.txt, prueba2.txt, prueba3.txt.
  ![1c](https://cloud.githubusercontent.com/assets/17281733/23804726/18651dd4-0589-11e7-9d05-1bcc5f3b4ba2.png)
  
   Se imprimen los nombres de los archivos que contienen la palabra “Carlos”
   ![1d](https://cloud.githubusercontent.com/assets/17281733/23804927/e16a2bac-0589-11e7-9f1d-44b8248554ff.png)
 

•	*simple_sort*

  Se ordena el contenido del archivo prueba.txt con el comando “sort”
  ![1e](https://cloud.githubusercontent.com/assets/17281733/23804978/101ad30c-058a-11e7-8160-3f502dc1a455.png)


•	*count_string_in_line*
  
  Cuenta el numero de líneas que contienen “si”. En el archivo de prueba, dichas líneas son la primera (sistema) y la ultima (Universidad,  Icesi)
  ![countstring](https://cloud.githubusercontent.com/assets/17281733/23805119/a3db5a80-058a-11e7-9552-509457e5245c.png)

 
•	last_lines

  Se imprimen las ultimas 2 lineas del archivo prueba.txt con el comando “tail”
  ![lastlines](https://cloud.githubusercontent.com/assets/17281733/23805150/c1407542-058a-11e7-9b2f-bdb46b071f41.png)

 

**PUNTO 2**

*Realice un script que a partir de un listado con no menos de dos direcciones ip, descargue en forma remota un libro del 
proyecto https://www.gutenberg.org/ en el directorio /tmp de cada equipo. El usuario operativos con contraseña operativos 
debe existir en los equipos. Presente capturas de pantalla relevantes como evidencias del funcionamiento.*


Para este ejercicio utilicé tres maquinas virtuales en mi portátil. Una de ellas ejecutaba el script. 
![3maquinas](https://cloud.githubusercontent.com/assets/17281733/23805214/f79e2b2a-058a-11e7-8062-dd2eb66feb0b.png)
 

El libro que se decidió descargar esta presente en el siguiente enlace: https://www.gutenberg.org/files/54286/54286-0.txt

![titulolibro](https://cloud.githubusercontent.com/assets/17281733/23805239/12b61f62-058b-11e7-9894-a5700c22521a.png)
 


*listado de direcciones ip (direccionesIP.txt)*
![direccionesip](https://cloud.githubusercontent.com/assets/17281733/23805278/3cb69242-058b-11e7-9ca1-9f0ab31e94e5.png)

 
*Script (script.sh)*
![script](https://cloud.githubusercontent.com/assets/17281733/23805320/692c05dc-058b-11e7-9808-4950d920579a.png)
 


*Ejecución del script*

En una de las maquinas virtuales se ejecutó el script
![ejecucionscript](https://cloud.githubusercontent.com/assets/17281733/23805393/aaf83828-058b-11e7-81e3-ced369a2c7a0.png)
 

*Resultado del script*

Como resultado de la ejecución del script, en las otras dos maquinas virtuales se descargó el libro y su contenido fue almacenado en el archivo libro.txt.
![libro1](https://cloud.githubusercontent.com/assets/17281733/23805426/d5b7b624-058b-11e7-800a-a328848bc5ce.png)

 
![libro2](https://cloud.githubusercontent.com/assets/17281733/23805449/f06f89f6-058b-11e7-92f6-e2d85a130ec0.png)


![evidenciadescarga](https://cloud.githubusercontent.com/assets/17281733/23805490/1504f486-058c-11e7-9185-ced65715f590.png)

 

**PUNTO 3**

*Cree un contenedor de debian en CentOS7 empleando LXC. Presente el listado de los comandos empleados y capturas de pantalla 
relevantes como evidencias del funcionamiento.*


Instalación de LXC 
 
![1](https://cloud.githubusercontent.com/assets/17281733/23805728/0cd63580-058d-11e7-885d-930f4c425f17.png)

![2](https://cloud.githubusercontent.com/assets/17281733/23805736/18574368-058d-11e7-91b3-63caf0b388e9.png)

![3](https://cloud.githubusercontent.com/assets/17281733/23805745/293b9b70-058d-11e7-8a04-953e59acfee3.png)

![4](https://cloud.githubusercontent.com/assets/17281733/23805752/32cbe410-058d-11e7-9531-c49674004b58.png)
 
 
Empezar el servicio LXC

![1](https://cloud.githubusercontent.com/assets/17281733/23805790/530a626a-058d-11e7-95b6-6c30d4973c85.png)
 
![2](https://cloud.githubusercontent.com/assets/17281733/23805825/75e74cda-058d-11e7-8417-d5a4f1090f72.png)

 
Verificar plantillas para contenedores

![1](https://cloud.githubusercontent.com/assets/17281733/23805853/8afaebe0-058d-11e7-8acf-361eb0517c79.png)


Creación del contenedor

![1](https://cloud.githubusercontent.com/assets/17281733/23805897/b46918a8-058d-11e7-8374-68636ff2df10.png)
 
![2](https://cloud.githubusercontent.com/assets/17281733/23805918/cad9667e-058d-11e7-982f-29b0ccd52d51.png)


Inicio del contenedor

![1](https://cloud.githubusercontent.com/assets/17281733/23805948/e00616c8-058d-11e7-8638-0e8a5703ea56.png)

![2](https://cloud.githubusercontent.com/assets/17281733/23805966/ebfac1ae-058d-11e7-9451-c678ca12ff11.png)
 


**REFERENCIAS**

•	*How to Install, Create and Manage LXC (Linux Containers) in RHEL/CentOS 7:*
  http://www.tecmint.com/install-create-run-lxc-linux-containers-on-centos/


