# **Fundamentos de Ingeniería de Software**
## **Tarea 01 Introducción a Git**

### **Nombre del alumno:** Alan Zenteno Paz  

### **Matricula:** 2203065778  

### **Descripción:**  
Este proyecto es una práctica básica de control de versiones utilizando Git y GitHub. Se centra en la creación de un programa sencillo en Java que imprime el mensaje "Hola Git". A lo largo de esta tarea, se aprende a inicializar un repositorio local, realizar commits, gestionar archivos a través de un archivo “.gitignore”, y finalmente, subir los cambios a un repositorio remoto en GitHub.

### **Objetivos:**  
- Familiarizarse con los comandos básicos de Git.
- Comprender el uso de archivos `.gitignore` para excluir archivos no deseados del control de versiones.
- Aprender a crear y gestionar un repositorio en GitHub.


### **Instrucciones de uso:**  


**Caso 1:** Tienes Java instalado 

- Abre una terminal o consola de comandos.
- Navega al directorio donde se encuentra el archivo HolaMundo.java. Puedes usar el comando cd para cambiar de directorio. Por ejemplo:  
  `cd /ruta/al/directorio`
- Compila el programa. Escribe el siguiente comando:  
  `javac HolaMundo.java`
- Esto generará un archivo llamado HolaMundo.class si no hay errores en el código.
- Ejecuta el programa. Usa el siguiente comando:  
  `java HolaMundo`
- Esto debería mostrar el mensaje que imprime tu programa.


**Caso 2:** No tienes Java instalado  

Si intentas ejecutar javac o java y obtienes un mensaje de error que dice que no se reconoce el comando, necesitarás instalar Java.  

**Descarga e instala Java:**  
- Ve al sitio web de Oracle o Adoptium para obtener el JDK (Java Development Kit).
  
**Configura las variables de entorno (si es necesario):**  
- En Windows, puede que necesites agregar el directorio bin del JDK a la variable de entorno PATH.

**Verifica la instalación:**  
- Abre una nueva terminal y escribe:  
  `java -version`
- Si se ve información sobre la versión de Java, significa que está instalado correctamente.


### **Comandos utilizados:**  

- **mkdir ProyectoEjemploGit:** Crea un nuevo directorio llamado ProyectoEjemploGit.
- **cd ProyectoEjemploGit:** Cambia al directorio ProyectoEjemploGit que se acaba de crear.
- **git init:** Inicializa un nuevo repositorio Git en el directorio actual. Esto crea un subdirectorio .git que contiene todos los archivos necesarios para el repositorio.
- **echo 'public class HolaMundo {...}' > HolaMundo.java:** Crea un archivo llamado HolaMundo.java y escribe un fragmento de código Java en él. Este comando sobrescribe cualquier contenido previo del archivo.
- **git add HolaMundo.java:** Agrega HolaMundo.java al área de preparación (staging area), lo que significa que está listo para ser incluido en el próximo commit.
- **git commit -m "Se agregó el programa de Hola Mundo en Java":** Crea un commit con el mensaje "Se agregó el programa de Hola Mundo en Java", registrando los cambios en el repositorio.
- **touch debug.log:** Crea un archivo vacío llamado debug.log. Si el archivo ya existe, no hace nada.
- **echo '*.log' > .gitignore:** Crea o sobrescribe el archivo .gitignore con el contenido *.log, indicando a Git que ignore todos los archivos con extensión .log.
- **git add .gitignore:** Agrega el archivo .gitignore al área de preparación.
- **git commit -m "Se agregó el archivo .gitignore":** Crea un commit con el mensaje "Se agregó el archivo .gitignore", registrando la inclusión del archivo de ignorar.
- **git add HolaMundo.java:** Agrega nuevamente HolaMundo.java al área de preparación. Esto es para incluir cambios realizados en el archivo después del primer commit.
- **git commit -m "Se actualizó el mensaje en HolaMundo.java":** Crea otro commit con el mensaje "Se actualizó el mensaje en HolaMundo.java", registrando los cambios realizados en HolaMundo.java.
- **git remote add origin <URL_DEL_REPOSITORIO>:** Agrega un repositorio remoto llamado origin que apunta a la URL que se proporcionó. Esto permite vincular el repositorio local con uno en un servicio de alojamiento como GitHub.
- **git push -u origin master:** Envía (push) los commits de la rama master al repositorio remoto origin. La opción -u establece una relación de seguimiento entre la rama local y la rama remota.


### **Notas sobre el archivo .gitignore:** 
 
Se creó el archivo .gitignore para evitar que ciertos archivos, como los archivos de log (por ejemplo, debug.log), sean rastreados por Git. Esto ayuda a mantener el repositorio limpio y evitar subir archivos innecesarios.  
Al ejecutar el programa, debería mostrarse el mensaje:  
**Hola Git**  
Para verificar que debug.log no se subió, puedes usar el comando:  
`git status`  
Si debug.log no aparece en la lista de archivos no rastreados, significa que se está ignorando correctamente.
