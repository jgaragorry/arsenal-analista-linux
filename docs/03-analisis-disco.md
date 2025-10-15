[⬅️ Volver al Inicio](../README.md)

# 3. Análisis de Espacio en Disco 💾

Una de las alertas más comunes es "disco lleno". Estas herramientas te permiten diagnosticar rápidamente el estado de tus particiones y "cazar" los archivos o directorios que consumen espacio indebidamente.

---

### **🔵 Clásico: `df -h`**
* **¿Qué hace?:** Muestra el uso de espacio en disco para todos los sistemas de archivos montados en un formato legible para humanos (`-h`).
* **Sintaxis y Ejemplo:** `df -h`
* **Salida Esperada:**
    > Una tabla que lista cada partición (`/`, `/boot`, etc.), su tamaño total, el espacio usado, el espacio disponible y el porcentaje de uso. Tu foco está en la columna `Use%`.

---

### **🟢 Moderno: `duf`**
* **¿Qué hace?:** Una utilidad para revisar el espacio en disco con una salida más limpia y organizada.
* **¿Por qué es mejor?:** **Claridad y organización**. La presentación visual de `duf` agrupa los dispositivos y usa colores, permitiéndote identificar la información relevante mucho más rápido.
* **Sintaxis y Ejemplo:** `duf`
* **Salida Esperada:**
    > Una tabla colorida y bien espaciada que es mucho más fácil de leer que la de `df`.

---

### **🔵 Clásico: `du -sh *`**
* **¿Qué hace?:** Calcula y muestra el tamaño de cada archivo y directorio en la ubicación actual. `-s` para resumir y `-h` para formato legible.
* **Sintaxis y Ejemplo:** Estando en un directorio que quieres investigar: `cd /var/log && du -sh *`
* **Salida Esperada:**
    > Una lista de los archivos y subdirectorios con su tamaño total al lado. Ejemplo: `4.5G syslog`.

---

### **🟢 Moderno: `ncdu`**
* **¿Qué hace?:** Analiza el uso de disco de un directorio y proporciona una interfaz interactiva para navegar y encontrar qué es lo que más espacio ocupa.
* **¿Por qué es mejor?:** Es una **herramienta de análisis, no solo un reporte**. `du` te dice el tamaño, `ncdu` te permite navegar interactivamente para descubrir *por qué* algo ocupa tanto espacio.
* **Sintaxis y Ejemplo:** `ncdu /var/log`
* **Salida Esperada:**
    > Primero, una pantalla de progreso mientras escanea. Luego, una lista de directorios y archivos ordenados por tamaño. Puedes usar las flechas para "entrar" en los directorios más pesados y seguir investigando hasta encontrar la causa raíz.

[⬅️ Volver al Inicio](../README.md)
