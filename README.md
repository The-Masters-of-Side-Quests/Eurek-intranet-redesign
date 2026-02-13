# 🧩 Rediseño de Intranet: Control System para Game Masters (Eurek)

[![Organization](https://img.shields.io/badge/Organization-The%20Masters%20of%20Side%20Quests-blue)](https://github.com/The-Masters-of-Side-Quests/)
[![Project Status](https://img.shields.io/badge/Status-Completed-success)](#)
[![Month](https://img.shields.io/badge/Date-December%202025-orange)](#)

A comprehensive redesign of the Eurek Game Master intranet, developed in December 2025 as part of the IronHack internship program. We focused on UX/UI and a minimalist aesthetic to optimize real-time game management and reduce cognitive load.

---

## 📝 Resumen del Proyecto

Durante nuestro periodo de prácticas en **Eurek**, asumimos el reto de transformar la herramienta interna que utilizan los **Game Masters** para la monitorización y control de las salas de Escape Room.

El objetivo principal fue pasar de una interfaz legacy a una plataforma moderna, minimalista, responsiva y optimizada para el uso en tiempo real.

---

## 🔍 Análisis del Problema (Legacy System)

Al iniciar las prácticas, realizamos una auditoría de la plataforma existente para identificar los puntos críticos que dificultaban la labor diaria de los **Game Masters**. Nos encontramos con una herramienta funcional, pero con importantes barreras de usabilidad que afectaban la eficiencia operativa:

* **Fricción en la Navegación (Selector de Juegos):**
    El acceso a las salas se gestionaba mediante un carrusel que ocupaba la totalidad de la pantalla, mostrando un solo juego a la vez. Este sistema obligaba al usuario a realizar un scroll innecesario y múltiples clics de navegación lateral; por ejemplo, para acceder a la séptima sala de una lista, el Game Master debía interactuar siete veces, un flujo ineficiente para una gestión rápida.

* **Arquitectura de Información Inconsistente:**
    La interfaz presentaba una disposición de menús y submenús poco intuitiva. La presencia de botones redundantes y una distribución de elementos sin una lógica de flujo de trabajo clara generaba una curva de aprendizaje elevada y fatiga visual durante las sesiones de juego.

* **Jerarquía Visual Deficiente:**
    El uso de tipografías desproporcionadamente grandes y elementos visuales con excesivo espacio negativo forzaba al usuario a realizar scroll constante para visualizar datos críticos que deberían estar disponibles de un solo vistazo.

* **Falta de Responsividad (Mobile Gap):**
    La ausencia de un diseño adaptativo limitaba el uso de la herramienta exclusivamente a ordenadores de escritorio, "atando" al Game Master a un puesto fijo e impidiendo la supervisión de las salas mientras se desplazaba por las instalaciones.

---

## 💡 Decisiones de Diseño y Soluciones UX

Adoptamos una estrategia **Mobile-First** para garantizar que el control de la sala sea fluido y reactivo, independientemente del dispositivo utilizado por el Game Master.

### 1. Sistema de Selección de Salas (Home)
- **El Reto:** Crear una vista escalable tanto para clientes con una sola sala como para aquellos con más de 30.
- **La Solución:** Implementamos una **cuadrícula estilo Instagram** basada en **Flip Cards**. Esto redujo drásticamente el tamaño de los contenedores, eliminando el scroll infinito y permitiendo una visión global. Además, integramos un buscador dinámico para agilizar el acceso en cuentas con gran volumen de juegos.
- **Jerarquía de Información:** Priorizamos los datos críticos (Estado, Tiempo y Porcentaje) en el frontal. La información administrativa (usuario, GM) se trasladó a una capa secundaria accesible mediante un icono de información con efecto *blur*.
- **Minimalismo Operativo:** Sustituimos etiquetas de texto por **indicadores cromáticos** (bolitas de estado) y un buscador expandible para maximizar el espacio útil.

### 2. Navegación Inteligente y Menús Dinámicos
Rediseñamos la arquitectura para que la interfaz "reaccione" proactivamente al estado del juego:
- **Navegación Condicional:** Implementamos un **menú flotante de gestión** vinculado al estado de la partida. Si no hay un juego en curso, el sistema oculta estas opciones de control para evitar errores operativos.
- **Adaptabilidad Desktop vs Mobile:** - En **Mobile**, centralizamos las opciones secundarias en un menú hamburguesa limpio.
    - En **Desktop**, diseñamos una **Sidebar interactiva** contraída que se expande mediante *hover*, optimizando el área de trabajo principal.
- **Header Adaptativo:** Durante la sesión, el nombre de la sala se integra en el header, proporcionando al Game Master una referencia constante y clara de su ubicación actual en el sistema.

### 3. Componentes y Accesibilidad
Diseñamos desde cero componentes que anteriormente dependían del sistema operativo o carecían de una identidad visual definida:

- **Modales Custom (UI/UX):** Sustituimos los diálogos nativos del navegador por modales minimalistas con estilos propios. Incluimos lógica de cierre mediante "X" y clic en el *overlay* exterior para una interacción más natural.
- **Gestión de Video (Cámaras):** Adaptamos la sección de monitorización a mobile, permitiendo visualización en cascada, actualización individual de feeds y modo a pantalla completa. Añadimos un selector rápido para saltar entre cámaras sin perder el flujo de juego.
- **Check Tools (Optimización de Diagnóstico):** Transformamos una herramienta de comprobación manual y unitaria en un panel de control masivo. Implementamos funciones de **selección múltiple**, botón de "comprobar todos" y reset general, integrando además un buscador específico para los elementos de la sala.
- **Accesibilidad y Control:** Utilizamos contornos con colores validados para el estado de los sensores (MQTT) y aplicamos **acordeones inteligentes** en la gestión de puzles para permitir una búsqueda visual ágil sin colapsar la pantalla.

> [!TIP]
> **[INSERTA AQUÍ GIF_O_IMAGEN_CHECKTOOLS.GIF]** > *Leyenda: Nueva interfaz de Check Tools con selección masiva y buscador.*

---

## 🛠️ Stack Tecnológico 

Para este rediseño y la implementación de las prácticas, trabajamos con las siguientes tecnologías:

| Área | Herramientas |
| :--- | :--- |
| **Diseño UI/UX** | Figma (Prototipado, Sistemas de diseño, Wireframing) |
| **Frontend** | HTML5, CSS3, JavaScript (ES6+) |
| **Arquitectura** | Mobile-First Strategy, Atomic Design principles |
| **Gestión** | Jira, Confluence, Trello |
| **Control de Versión** | Git, GitHub (GitHub Organizations) |
---

## 👥 Equipo: The Masters of Side Quests

Este proyecto fue desarrollado de forma colaborativa por:

- **Aïda** - [Tu Rol: ej. Fullstack Dev / UI Designer] - [@AidaG91](https://github.com/AidaG91)
- **Wil** - [Rol de Wil: ej. Frontend Dev / UX Specialist] - [@wilpipe](https://github.com/wilpipe)

---

## 🧠 Aprendizajes Clave

Durante este mes de inmersión en **Eurek**, no solo mejoramos nuestras habilidades técnicas, sino que desarrollamos competencias críticas para el entorno laboral:

* **Gestión de la Confidencialidad:** Aprendimos a trabajar bajo acuerdos de confidencialidad (NDA), comprendiendo la importancia de proteger la propiedad intelectual de la empresa.
* **Comunicación Cliente-Developer:** Realizamos sesiones de feedback con los responsables del proyecto para validar que nuestras decisiones de diseño se alineaban con la lógica de negocio.
* **Pair Programming:** @wilpipe y yo trabajamos de forma síncrona, mejorando la calidad del diseño y la velocidad de resolución de problemas técnicos.
* **Pensamiento Crítico:** No nos limitamos a rediseñar; cuestionamos la herramienta actual para proponer soluciones que realmente ahorran tiempo al usuario final.

---

## 📄 Nota de Confidencialidad

Este repositorio cumple una función exclusivamente de **documentación técnica y portfolio**. 

Debido al acuerdo de confidencialidad (NDA) con la empresa **Eurek**, el código fuente original es privado y no se encuentra disponible en este repositorio. Para proteger la propiedad intelectual de la empresa, los recursos visuales aquí mostrados han sido **anonimizados**: se han eliminado logotipos, se ha modificado la paleta de colores original y se han alterado datos sensibles, manteniendo únicamente la estructura lógica y funcional del diseño desarrollado durante el programa de **IronHack 2025**.