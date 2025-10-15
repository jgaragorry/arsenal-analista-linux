[⬅️ Volver al Inicio](../README.md)

# 4. Análisis de Logs 📜

Los logs son el diario de tu sistema. Aprender a leerlos de manera eficiente es la habilidad clave para diagnosticar cualquier problema. Las herramientas modernas transforman esta tarea de buscar una aguja en un pajar a un análisis forense preciso.

---

### **🔵 Clásico: `tail -f` y `grep`**
* **¿Qué hacen?:** `tail -f` te permite ver un log en tiempo real. `grep` te permite buscar texto (como "ERROR") dentro de un archivo.
* **Sintaxis y Ejemplo:**
    ```bash
    # Ver un log en vivo
    tail -f /var/log/nginx/access.log

    # Buscar errores en un log
    grep "ERROR" /var/log/app/application.log
    ```
* **Salida Esperada:**
    > `tail -f` mostrará las últimas líneas del archivo y luego imprimirá cada nueva línea que se añada. `grep` mostrará únicamente las líneas que contengan la palabra "ERROR".

---

### **🟢 Moderno (Systemd): `journalctl`**
* **¿Qué hace?:** Es la herramienta estándar para consultar los logs en la mayoría de las distribuciones modernas de Linux (Ubuntu, Debian, CentOS 8+, etc.). Centraliza los logs de todas las aplicaciones y del sistema.
* **¿Por qué es superior?:** Permite un **filtrado estructurado**. Puedes filtrar por unidad de servicio (`-u`), por tiempo (`--since "10 min ago"`) o por nivel de severidad (`-p err`) de forma nativa, algo mucho más potente que buscar texto plano.
* **Sintaxis y Ejemplo:**
    ```bash
    # Ver los logs del servicio nginx y seguir en tiempo real
    journalctl -u nginx.service -f
    ```
* **Salida Esperada:**
    > Un flujo de logs específico del servicio Nginx. Las líneas están coloreadas según su prioridad (rojo para errores).

---

### **🚀 Nueva Generación (Múltiples Archivos): `multitail`**
* **¿Qué hace?:** Permite ver múltiples archivos de log en tiempo real dividiendo la pantalla de la terminal.
* **¿Por qué es útil?:** Es indispensable para la **correlación de eventos**. Te permite ver la petición de un usuario en el log del servidor web y el error que esa petición generó en el log de la aplicación, todo al mismo tiempo.
* **Sintaxis y Ejemplo:**
    ```bash
    multitail /var/log/nginx/access.log /var/log/app/application.log
    ```
* **Salida Esperada:**
    > Tu terminal se dividirá en dos paneles. El panel superior mostrará el `access.log` y el inferior el `application.log`, ambos actualizándose en tiempo real.

[⬅️ Volver al Inicio](../README.md)
