# **Fundamentos de Ingeniería de Software**
## **Tarea 01**

### **Nombre del alumno:** daniel monroy marcelo

### **Matricula:** 2203065803

Aquí tienes el texto **reescrito**, más claro y fluido, pero conservando toda la información que describe:

---

### **Descripción:**

Este proyecto consiste en una práctica introductoria al uso de Git y GitHub. El objetivo es crear un programa sencillo en Java que imprima el mensaje **"Hola Git"**, mientras se aprende a manejar las funciones básicas de control de versiones. Durante la actividad se realiza la creación de un repositorio local, la ejecución de commits, el uso de un archivo `.gitignore` para excluir archivos no deseados, y finalmente, la publicación del proyecto en un repositorio remoto en GitHub.

---

### **Objetivos:**

* Dominar los comandos esenciales de Git.
* Comprender para qué sirve el archivo `.gitignore` y cómo utilizarlo para evitar subir archivos innecesarios.
* Conocer el proceso para crear y administrar un repositorio en GitHub.

---

### **Instrucciones de uso:**

## **Caso 1: Ya tienes Java instalado**

1. Abre una terminal.
2. Entra al directorio donde está el archivo **HolaMundo.java** usando:

   ```bash
   cd /ruta/al/directorio
   ```
3. Compila el programa con:

   ```bash
   javac HolaMundo.java
   ```

   Esto generará el archivo **HolaMundo.class** si no hay errores.
4. Ejecuta el programa escribiendo:

   ```bash
   java HolaMundo
   ```

   Deberías ver el mensaje que imprime tu código.

---

## **Caso 2: No tienes Java instalado**

Si al intentar usar `javac` o `java` aparece un error indicando que el comando no existe, necesitas instalar Java.

### **Instalar Java (JDK):**

* Descárgalo desde el sitio oficial de Oracle o desde Adoptium.

### **Configurar variables de entorno (solo si es necesario):**

* En Windows, tal vez debas agregar la ruta del directorio `bin` del JDK a la variable `PATH`.

### **Verificar instalación:**

En una nueva terminal escribe:

```bash
java -version
```

Si se muestra información sobre la versión instalada, Java se configuró correctamente.

---

### **Comandos utilizados:**

* **mkdir ProyectoEjemploGit:** crea un directorio llamado ProyectoEjemploGit.
* **cd ProyectoEjemploGit:** accede al directorio recién creado.
* **git init:** inicializa un repositorio Git creando la carpeta `.git`.
* **echo 'public class HolaMundo {...}' > HolaMundo.java:** genera el archivo HolaMundo.java con un fragmento de código Java (sobrescribe si ya existía).
* **git add HolaMundo.java:** agrega el archivo al área de preparación.
* **git commit -m "Se agregó el programa de Hola Mundo en Java":** registra el archivo en el repositorio local.
* **touch debug.log:** crea un archivo vacío llamado debug.log.
* **echo '*.log' > .gitignore:** crea o reemplaza `.gitignore` para ignorar todos los archivos con extensión `.log`.
* **git add .gitignore:** prepara el archivo `.gitignore` para su commit.
* **git commit -m "Se agregó el archivo .gitignore":** registra el archivo .gitignore.
* **git add HolaMundo.java:** vuelve a preparar HolaMundo.java tras realizar cambios.
* **git commit -m "Se actualizó el mensaje en HolaMundo.java":** registra la actualización realizada.
* **git remote add origin <URL_DEL_REPOSITORIO>:** vincula el repositorio local con el repositorio remoto en GitHub.
* **git push -u origin master:** envía los commits a GitHub y establece seguimiento entre ambas ramas.

---

### **Notas sobre el archivo .gitignore:**

El archivo `.gitignore` se creó para evitar que archivos innecesarios, como los archivos de registro (`debug.log`), sean incluidos en el repositorio. Esto ayuda a mantener el proyecto limpio y profesional.
Después de ejecutar el programa, deberías ver el mensaje:
**Hola Git**

Para comprobar que `debug.log` está siendo ignorado, puedes usar:

```bash
git status
```

Si no aparece en la lista de archivos sin seguimiento, el `.gitignore` está funcionando correctamente.

---


