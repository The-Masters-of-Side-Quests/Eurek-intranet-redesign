# 🧩 Rediseño de Intranet: Control System para Game Masters (Eurek)

[![Organization](https://img.shields.io/badge/Organization-The%20Masters%20of%20Side%20Quests-blue)](https://github.com/The-Masters-of-Side-Quests/)
[![Project Status](https://img.shields.io/badge/Status-Completed-success)](#)
[![Month](https://img.shields.io/badge/Date-December%202025-orange)](#)

A comprehensive redesign of the Eurek Game Master intranet, developed in December 2025 as part of the IronHack internship program. We focused on UX/UI and a minimalist aesthetic to optimize real-time game management and reduce cognitive load.

---

## 📝 Resumen del Proyecto

Durante nuestro periodo de prácticas en **Eurek**, asumimos el reto de transformar la herramienta interna que utilizan los **Game Masters** para la monitorización y control de las salas de Escape Room.

El objetivo principal fue pasar de una interfaz legacy a una plataforma moderna, intuitiva y optimizada para el uso en tiempo real, donde cada segundo cuenta.

---

## 🔍 Análisis del Problema (Legacy System)

Al iniciar las prácticas, realizamos una auditoría de la plataforma existente (**TheMasterKI**), identificando puntos críticos que afectaban la operatividad de los Game Masters:

- **Jerarquía Visual Deficiente:** Tipografías excesivamente grandes (16px) y elementos redundantes que forzaban un scroll innecesario.
- **Falta de Responsividad:** Una herramienta web no adaptada a dispositivos móviles, limitando al Game Master a un puesto fijo.
- **Redundancia de Datos:** Confusión entre "Acciones" y "Secuencias" con interfaces idénticas pero funciones distintas.

---

## 💡 Decisiones de Diseño y Soluciones UX

Adoptamos una estrategia **Mobile-First** para garantizar que el control de la sala sea fluido desde cualquier dispositivo.

### 1. Sistema de Selección de Salas (Home)
- **El Reto:** Adaptar la vista para clientes con 1 sala y clientes con más de 30.
- **Solución:** Implementamos una **cuadrícula estilo Instagram** con **Flip Cards** que ocultan la información secundaria (Game Master logueado, usuario) tras un icono de información, manteniendo el foco en lo vital: **Estado, Tiempo y Porcentaje**.
- **Minimalismo:** Sustitución de etiquetas de texto por indicadores cromáticos (bolitas de estado) y buscadores expandibles.
- Problema de los menús mezclados --> hablar de la solución

> [!TIP]
> **[INSERTA AQUÍ GIF_HOME_FIGMA.GIF]** > *Leyenda: Prototipo de selección de salas con buscador dinámico y flip-cards.*

### 2. Panel de Gestión de Juego
- **Acordeones Inteligentes:** Rediseñamos las secciones de Acciones y Secuencias usando acordeones para colapsar la información.
- **Búsqueda Visual Ágil:** Mantuvimos las imágenes de los puzles visibles incluso con el acordeón cerrado, permitiendo al Game Master identificar el puzle al instante.
- **Header Dinámico:** Reducción del branding al hacer scroll para maximizar el espacio de trabajo en pantallas pequeñas.

> [!TIP]
> **[INSERTA AQUÍ CAPTURA_GESTION_MOBILE.PNG]** > *Leyenda: Vista de gestión de partida con sistema de acordeones y menú optimizado.*

### 3. Componentes y Accesibilidad
- **Modales Custom:** Sustituimos los diálogos de sistema por modales minimalistas con cierre por clic exterior, mejorando la usabilidad.
- **Colores Accesibles:** Implementamos contornos de tarjetas con colores validados para accesibilidad en el control de sensores (MQTT).
- **Lógica de Cámaras:** Unificamos el flujo de video en "Vistas" (global) y "Cámaras" (individual) para una supervisión eficiente.


### 🖼️ Preview del Dashboard
> [!TIP]
> [INSERTAR AQUÍ UNA CAPTURA DE TU FIGMA (Desktop)]
> *Leyenda: Vista principal del panel de control con cronómetros y gestión de pistas.*

### 📱 Adaptabilidad Mobile
> [!TIP]
> [INSERTAR AQUÍ UNA CAPTURA DE TU FIGMA (Mobile)]
> *Leyenda: El Game Master ahora puede controlar la sala desde cualquier lugar de la empresa.*

---

## 🛠️ Stack Tecnológico Proyectado

Para este rediseño y la implementación de las prácticas, trabajamos con las siguientes tecnologías:

- **Diseño:** Figma (Prototipado de alta fidelidad y flujos de usuario).
- **Frontend:** [Ej: React.js, Tailwind CSS]
- **Tiempo Real:** [Ej: WebSockets / Socket.io] para la sincronización de cronómetros.
- **Metodología:** Agile (Daily checks y gestión de tareas en JIRA/Confluence).
- **Control de Versiones:** Git & GitHub (Workflows profesionales).

---

## 🚀 Retos Técnicos y Soluciones

### 1. Sincronización en tiempo real
**Reto:** Mantener el tiempo de la sala y los eventos sincronizados entre el servidor y la interfaz del Game Master sin latencia.
**Solución:** [Explica brevemente cómo lo hicisteis, ej: Implementación de un estado global eficiente].

### 2. Gestión de múltiples salas
**Reto:** Permitir que un solo Game Master pueda supervisar varias salas simultáneamente sin perder detalle.
**Solución:** Creación de una arquitectura de componentes modulares y escalables.

---

## 👥 Equipo: The Masters of Side Quests

Este proyecto fue desarrollado de forma colaborativa por:

- **Aïda** - [Tu Rol: ej. Fullstack Dev / UI Designer] - [@AidaG91](https://github.com/AidaG91)
- **Wil** - [Rol de Wil: ej. Frontend Dev / UX Specialist] - [@wilpipe](https://github.com/wilpipe)

---

## 📄 Nota de Confidencialidad
Este repositorio sirve como **documentación técnica y portfolio**. Por motivos de confidencialidad (NDA) con la empresa Eurek, el código fuente original no está disponible públicamente. Las imágenes mostradas son prototipos de diseño propiedad de los autores desarrollados durante el programa de IronHack 2025..