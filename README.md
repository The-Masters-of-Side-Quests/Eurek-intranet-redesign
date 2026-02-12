# 🧩 Rediseño de Intranet: Control System para Game Masters

[![Organization](https://img.shields.io/badge/Organization-The%20Masters%20of%20Side%20Quests-blue)](https://github.com/TU_ORGANIZACION)
[![Project Status](https://img.shields.io/badge/Status-Completed-success)](#)

## 📝 Resumen del Proyecto

Durante nuestro periodo de prácticas en **Eurek**, asumimos el reto de transformar la herramienta interna que utilizan los **Game Masters** para la monitorización y control de las salas de Escape Room.

El objetivo principal fue pasar de una interfaz legacy a una plataforma moderna, intuitiva y optimizada para el uso en tiempo real, donde cada segundo cuenta.

---

## 🎨 El Diseño (UX/UI)

Debido a la naturaleza confidencial del código fuente, mostramos aquí el proceso de diseño y la arquitectura de información desarrollada en **Figma**.

### 🖼️ Preview del Dashboard
> [!TIP]
> [INSERTAR AQUÍ UNA CAPTURA DE TU FIGMA (Desktop)]
> *Leyenda: Vista principal del panel de control con cronómetros y gestión de pistas.*

### 📱 Adaptabilidad Mobile
> [!TIP]
> [INSERTAR AQUÍ UNA CAPTURA DE TU FIGMA (Mobile)]
> *Leyenda: El Game Master ahora puede controlar la sala desde cualquier lugar de la empresa.*

**Mejoras clave implementadas:**
- **Reducción de carga cognitiva:** Simplificación de menús para situaciones de alta tensión.
- **Jerarquía visual:** Priorización de alertas y estado de los sensores de la sala.
- **Flujo de Pistas:** Optimización del sistema de envío de mensajes a los jugadores (reducción de pasos).

---

## 🛠️ Stack Tecnológico Proyectado

Para este rediseño y la implementación de las prácticas, trabajamos con las siguientes tecnologías:

- **Frontend:** [Ej: React.js, Tailwind CSS]
- **Tiempo Real:** [Ej: WebSockets / Socket.io] para la sincronización de cronómetros.
- **Diseño:** Figma (Prototipado de alta fidelidad).
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

- **Nombre del Usuario** - [Tu Rol: ej. Fullstack Dev / UI Designer] - [@TuUsuario](https://github.com/TuUsuario)
- **Wil** - [Rol de Wil: ej. Frontend Dev / UX Specialist] - [@WilUsuario](https://github.com/WilUsuario)

---

## 📄 Nota de Confidencialidad
Este repositorio sirve como **documentación técnica y portfolio**. Por motivos de confidencialidad (NDA) con la empresa Eurek, el código fuente original no está disponible públicamente. Las imágenes mostradas son prototipos de diseño propiedad de los autores.