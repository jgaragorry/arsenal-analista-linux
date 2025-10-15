[⬅️ Volver al Inicio](../README.md)

# 2. Listado y Visualización de Archivos 📂

Navegar por el sistema de archivos es una tarea diaria. Estas herramientas modernizan la forma en que listas y visualizas el contenido de los archivos, ahorrando tiempo y evitando errores.

---

### **🔵 Clásico: `ls -l`**
* **¿Qué hace?:** Lista el contenido de un directorio en formato largo, mostrando permisos, propietario, tamaño y fecha de modificación.
* **Sintaxis y Ejemplo:** `ls -l /var/log`
* **Salida Esperada:**
    > `-rw-r----- 1 syslog adm 12345 Oct 15 20:00 syslog`

---

### **🟢 Moderno: `exa -l --icons`**
* **¿Qué hace?:** Un reemplazo moderno de `ls` con mejor formato, colores y características adicionales.
* **¿Por qué es mejor?:** La **información es más visual** gracias a los colores, iconos (con Nerd Fonts) y su integración nativa con Git, que muestra el estado de los archivos en un repositorio.
* **Sintaxis y Ejemplo:** `exa -l --icons /var/log`
* **Salida Esperada:**
    > Una lista similar a `ls` pero con colores e iconos que facilitan la identificación de tipos de archivo.

---

### **🔵 Clásico: `cat [archivo]`**
* **¿Qué hace?:** Muestra el contenido completo de un archivo en la salida estándar (la terminal).
* **Sintaxis y Ejemplo:** `cat /etc/nginx/nginx.conf`
* **Salida Esperada:**
    > El texto plano del archivo, sin ningún tipo de formato.

---

### **🟢 Moderno: `bat [archivo]`**
* **¿Qué hace?:** Muestra el contenido de un archivo con resaltado de sintaxis, numeración de líneas y paginación automática.
* **¿Por qué es mejor?:** El **resaltado de sintaxis** es revolucionario. Previene errores de interpretación al leer archivos de configuración o scripts, mostrando directivas, valores y comentarios en diferentes colores.
* **Sintaxis y Ejemplo:** `bat /etc/nginx/nginx.conf`
* **Salida Esperada:**
    > El contenido del archivo formateado con colores, como si lo vieras en un editor de código profesional.

[⬅️ Volver al Inicio](../README.md)
