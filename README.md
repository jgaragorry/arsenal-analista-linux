#  Arsenal del Analista Linux Moderno 🚀

![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)
![Last Commit](https://img.shields.io/github/last-commit/tu-usuario/arsenal-analista-linux)
![Repo Stars](https://img.shields.io/github/stars/tu-usuario/arsenal-analista-linux?style=social)

**Una guía curada de comandos de terminal para el monitoreo y diagnóstico de sistemas Linux, desde las herramientas clásicas universales hasta sus reemplazos modernos y superiores.**

---

### ¿Por qué existe este repositorio?

En el mundo de las operaciones de TI, la velocidad y la precisión son cruciales. Este repositorio nace de la necesidad de tener a mano una guía de referencia rápida, didáctica y moderna que no solo liste comandos, sino que **explique su propósito, muestre su uso y justifique por qué las herramientas de nueva generación nos hacen mejores profesionales.**

### ¿A quién va dirigido?

Este arsenal está forjado para:
* 👨‍🎓 **Estudiantes y Principiantes:** Que buscan una base sólida y las mejores prácticas desde el primer día.
* 👨‍💻 **Analistas y SysAdmins Junior:** Que necesitan una referencia rápida y fiable para sus tareas diarias.
* 👩‍🚀 **Profesionales con Experiencia:** Que desean actualizar su caja de herramientas y descubrir alternativas más eficientes a los comandos clásicos.
* 🕵️‍♂️ **Reclutadores y Líderes Técnicos:** Para evaluar el conocimiento y la familiaridad de un candidato con el ecosistema de herramientas moderno.

### La Historia Detrás del Arsenal

Este proyecto surgió de una necesidad real: preparar a un colega para una entrevista de trabajo en un rol de monitoreo de Nivel 1. La pregunta fue simple: "¿Qué comandos necesito saber?". La respuesta evolucionó de una simple lista a esta guía completa que compara lo clásico con lo moderno, convirtiéndose en un recurso para toda la comunidad.

---

## 🧭 Contenido del Arsenal

Navega a través de las guías detalladas para dominar cada área del análisis de sistemas.

* **[💻 Monitoreo de Procesos y Recursos](./docs/01-monitoreo-recursos.md)**
    > Aprende a usar `top`, `htop` y `btop` para obtener una visión completa del rendimiento de tu sistema.

* **[📂 Listado y Visualización de Archivos](./docs/02-gestion-archivos.md)**
    > Descubre cómo `exa` y `bat` revolucionan la forma en que interactúas con archivos y directorios.

* **[💾 Análisis de Espacio en Disco](./docs/03-analisis-disco.md)**
    > Domina `df`, `du`, `duf` y `ncdu` para nunca más ser sorprendido por una alerta de "disco lleno".

* **[📜 Análisis de Logs](./docs/04-analisis-logs.md)**
    > Conviértete en un experto forense de logs con `tail`, `grep`, `journalctl` y `multitail`.

---

### 🛠️ Instalación Rápida de Herramientas Modernas

Para instalar la mayoría de las herramientas modernas en sistemas basados en Debian/Ubuntu, puedes usar este único comando:

```bash
sudo apt update && sudo apt install htop btop exa bat duf ncdu multitail
