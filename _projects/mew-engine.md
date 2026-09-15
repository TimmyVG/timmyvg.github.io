---
title: MEW Engine
description: MEW Engine es un motor gráfico 3D desarrollado desde cero en C++17 y OpenGL
layout: project
image: /assets/img/Motor.png
role: Programador
engine: OpenGL
tags: [motor,opengl,c++]
order: 2
lang: es
---


El motor combina **ECS, multithreading, gestión de recursos, renderizado diferido y múltiples técnicas de iluminación y postprocesado**.

### ⚙️ Características

* **ECS** para la gestión de entidades y componentes.
* **OpenGL 4.6** mediante una capa de abstracción.
* **Forward & Deferred Rendering**.
* **Shadow Mapping** para sombras dinámicas.
* **SSAO** para mejorar la profundidad de las escenas.
* **Framebuffer & Render-to-Texture** para efectos de postprocesado.
* **HDR** y procesamiento de imagen.
* **Displacement Mapping**.
* **Carga de assets mediante Assimp**.
* **Sistema de Jobs y multithreading**.
* **Integración con Bullet Physics**.
* Herramientas de edición mediante **gizmos**.

---

{% include embed/youtube.html id='lJ-qqhkakpk' %}

## 💡 Renderizado dinámico

El motor permite trabajar tanto con **Forward Rendering** como con **Deferred Rendering**, utilizando diferentes pases de renderizado para gestionar las luces y materiales de la escena.


**Luces dinámicas + Shadow Mapping**

Las sombras se generan mediante **render-to-texture**, creando mapas de profundidad desde la perspectiva de las luces y utilizándolos posteriormente durante el proceso de iluminación.

---

## 🌑 Screen Space Ambient Occlusion



**SSAO aplicado en tiempo real**

El motor implementa **Ambient Occlusion y Screen Space Ambient Occlusion (SSAO)** para añadir información de oclusión en las zonas donde la geometría se encuentra próxima, aumentando la sensación de profundidad y contacto entre objetos.

---

## 🧩 Arquitectura

El motor está construido alrededor de un **Entity Component System**, separando las entidades de sus datos y de la lógica que los procesa.

Esto permite que los diferentes sistemas del motor trabajen sobre los componentes que necesitan sin acoplar directamente la lógica de juego con el renderer.

La arquitectura también incorpora un **sistema de Jobs** para ejecutar tareas de forma paralela y aprovechar los diferentes núcleos de la CPU.

---

## 🛠️ Tecnologías

`C++17` · `OpenGL 4.6` · `ECS` · `GLSL` · `CMake` · `Conan` · `Assimp` · `Bullet Physics`
