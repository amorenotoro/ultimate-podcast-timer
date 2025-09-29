# Ultimate Podcast Timer

![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![TailwindCSS](https://img.shields.io/badge/Tailwind_CSS-38B2AC?style=for-the-badge&logo=tailwind-css&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![Firebase](https://img.shields.io/badge/Firebase-FFCA28?style=for-the-badge&logo=firebase&logoColor=black)

<br>

<details>
<summary>🇪🇸 Ver descripción en Español</summary>

## 📖 Descripción del Proyecto

Este proyecto nació de una necesidad real surgida de mi experiencia en el mundo de la radio y el podcasting. `Ultimate Podcast Timer` es una herramienta colaborativa en tiempo real para la gestión de pautas y minutados durante la grabación de un podcast.

Como comunicador, sé que el tiempo y la estructura son cruciales. El objetivo de este proyecto era aplicar mis habilidades técnicas para crear una solución web sencilla que resolviera un problema recurrente en el flujo de trabajo de nuestro equipo.

## 🎯 El Problema que Resuelve

Durante la grabación de nuestro podcast, necesitábamos una forma sencilla y sincronizada de marcar los momentos clave (cambios de tema, puntos importantes, errores a editar). Esta lista de "hitos" con su minutaje exacto es un documento vital que se entrega al editor de audio. Hacerlo manualmente era ineficiente y propenso a errores.

Esta herramienta centraliza ese proceso, permitiendo que cualquier miembro del equipo añada notas al cronómetro compartido, generando un desglose perfecto para la postproducción y facilitando enormemente el trabajo de nuestro editor.

## ✨ Características Principales

-   **Cronómetro Sincronizado en Tiempo Real:** Utilizando Firebase, el temporizador es idéntico para todos los usuarios que tengan la aplicación abierta, garantizando que todos los hitos se registran sobre la misma línea de tiempo.
-   **Gestión de Hitos Colaborativa:** Cualquier participante en la sesión puede añadir notas o "hitos" de texto al minutaje actual. El último hito añadido se resalta para facilitar su seguimiento.
-   **Interfaz Sencilla y Enfocada:** La UI está diseñada para ser minimalista y funcional, sin distracciones, permitiendo a los locutores centrarse en lo importante: el contenido.
-   **Controles Esenciales:** Funciones de Start, Stop y Reset, todas sincronizadas para el grupo.

## 💡 El Reto Técnico

La mayor complejidad del proyecto era conseguir que el temporizador fuese una entidad única y sincronizada para múltiples clientes (navegadores) de forma simultánea.

Para resolverlo, utilicé la **Realtime Database de Firebase**. El estado del temporizador (startTime, running, difference) se almacena en la base de datos, y los clientes se suscriben a sus cambios, asegurando una sincronización robusta y con una latencia mínima.

## 🛠️ Stack Tecnológico

-   **Frontend:** HTML5, Tailwind CSS, JavaScript (ES6 Modules).
-   **Backend & Realtime Sync:** Firebase (Realtime Database).
-   **Plataforma:** Aplicación web estática.

## 🚀 Cómo Utilizarlo

1.  Clona este repositorio en tu máquina local.
2.  Abre el archivo `index.html` en cualquier navegador web moderno.
3.  ¡Listo! Puedes abrirlo en varias ventanas o dispositivos para ver la sincronización en acción.

> **Nota de Producción:** La configuración de Firebase está expuesta en el código cliente para facilitar la demostración. En un entorno de producción, las claves se gestionarían de forma segura a través de un backend o con reglas de seguridad más estrictas.

</details>

<hr>

## 📖 Project Description

This project was born from a real need I identified during my time in the radio and podcasting industry. `Ultimate Podcast Timer` is a real-time, collaborative tool designed to manage timestamps and show notes during a podcast recording session.

As a communicator, I know that time and structure are crucial. The goal of this project was to apply my technical skills to build a simple web solution that solves a recurring problem in our team's workflow.

## 🎯 The Problem It Solves

During our podcast recordings, we needed a simple, synchronized way to bookmark key moments (topic changes, important points, mistakes to be edited out). This list of "milestones" with their exact timestamps is a vital document for our audio editor. Doing this manually was inefficient and error-prone.

This tool centralizes that process, allowing any team member to add notes to a shared, live timer. This generates a perfect breakdown for the post-production phase, making our editor's job significantly easier.

## ✨ Key Features

-   **Real-Time Synchronized Timer:** Using Firebase, the timer is identical for all users with the application open, ensuring all milestones are logged against the same timeline.
-   **Collaborative Milestone Management:** Any participant in the session can add text notes or "milestones" at the current timestamp. The latest milestone is highlighted for easy tracking.
-   **Simple and Focused UI:** The interface is designed to be minimalist and functional, eliminating distractions and allowing hosts to focus on what matters: the content.
-   **Essential Controls:** Start, Stop, and Reset functions, all synchronized across the group.

## 💡 The Technical Challenge

The main complexity of this project was to make the timer a single, synchronized entity across multiple clients (browsers) simultaneously.

To solve this, I used **Firebase's Realtime Database**. The timer's state (startTime, running, difference) is stored in the database. Clients don't just calculate time locally; they subscribe to changes in that database, ensuring a robust and low-latency synchronization. The same principle applies to the list of milestones.

## 🛠️ Tech Stack

-   **Frontend:** HTML5, Tailwind CSS, JavaScript (ES6 Modules).
-   **Backend & Realtime Sync:** Firebase (Realtime Database).
-   **Platform:** Static Web Application.

## 🚀 How to Use

1.  Clone this repository to your local machine.
2.  Open the `index.html` file in any modern web browser.
3.  That's it! You can open it in multiple windows or on different devices to see the real-time synchronization in action.

> **Production Note:** The Firebase configuration is exposed on the client-side for the purpose of demonstrating this personal project. In a real production environment, API keys and database security would be managed securely, either through a backend service or with stricter database security rules to control access.
