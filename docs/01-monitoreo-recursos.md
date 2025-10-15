[⬅️ Volver al Inicio](../README.md)

# 1. Monitoreo de Procesos y Recursos del Sistema 💻

Esta sección se enfoca en las herramientas para obtener una visión en tiempo real del rendimiento de tu servidor, identificando cuellos de botella y procesos que consumen recursos excesivos.

---

### **🔵 Clásico: `top`**
* **¿Qué hace?:** Muestra una vista en tiempo real de los procesos del sistema, ordenados por defecto según el consumo de CPU. Es la herramienta de diagnóstico fundamental.
* **Sintaxis y Ejemplo:** Simplemente ejecuta `top` en la terminal.
    ```bash
    top
    ```
* **Salida Esperada:**
    > Una tabla de procesos que se actualiza constantemente. Las columnas clave son **`PID`** (ID del Proceso), **`%CPU`** (Uso de CPU) y **`%MEM`** (Uso de Memoria). Te fijarás en los procesos que aparecen en las primeras filas.

---

### **🟢 Moderno: `htop`**
* **¿Qué hace?:** Es un visor de procesos interactivo y una mejora visual sobre `top`.
* **¿Por qué es mejor?:** Es **interactivo y visual**. Permite desplazarse vertical y horizontalmente, matar procesos con una tecla (`F9`) y ver los procesos en forma de árbol (`F5`), lo que facilita entender las dependencias.
* **Sintaxis y Ejemplo:**
    ```bash
    htop
    ```
* **Salida Esperada:**
    > Una interfaz mucho más clara que `top`, con barras de uso para cada núcleo de CPU, memoria RAM y Swap. Los procesos están coloreados y puedes navegar por la lista con las flechas del teclado.

---

### **🚀 Nueva Generación: `btop`**
* **¿Qué hace?:** Un completo "dashboard" de recursos del sistema que muestra CPU, memoria, red, discos y procesos en una sola pantalla.
* **¿Por qué es superior?:** Es una **herramienta unificada**. Mientras `htop` se centra en los procesos, `btop` te da una visión 360° que te permite correlacionar un pico de CPU con un aumento en la escritura de disco o el tráfico de red, todo sin cambiar de herramienta. Soporta navegación con ratón.
* **Sintaxis y Ejemplo:**
    ```bash
    btop
    ```
* **Salida Esperada:**
    > Una interfaz gráfica en la terminal con gráficos históricos para todos los recursos principales.

[⬅️ Volver al Inicio](../README.md)
