# 🧠 Chat Indecision App

Una aplicación de práctica desarrollada con **Vue 3 + TypeScript**, donde puedes hacerle preguntas a una "inteligencia indecisa" y recibir respuestas tipo **sí/no**, acompañadas de un **GIF temático**. Ideal para aprender sobre componentes, composables, props y organización de proyectos modernos en Vue.

---

## 🚀 Características

- ✅ Preguntas abiertas con respuestas aleatorias tipo "sí" o "no"
- 🎬 GIFs dinámicos según la respuesta
- 🧩 Componentes reutilizables
- 🧠 Composables para lógica desacoplada
- 📦 Comunicación por props entre componentes
- 🛡️ Interfaces TypeScript para tipado seguro
- ⚡️ Scroll automático al recibir nuevos mensajes

---

## 🖼️ Vista previa

> *Próximamente: puedes agregar capturas de pantalla aquí para mostrar la interfaz.*

---

## 🧱 Estructura del proyecto

```bash
src/
├── components/       # Componentes visuales como ChatBubble
├── composables/      # Lógica reutilizable (e.g. manejo de API)
├── helpers/          # Funciones auxiliares
├── interfaces/       # Tipos e interfaces TypeScript
├── views/            # Vistas principales
├── App.vue           # Componente raíz
└── main.ts           # Punto de entrada
```

---

## 🛠️ Tecnologías utilizadas

- [Vue 3](https://vuejs.org/)
- [TypeScript](https://www.typescriptlang.org/)
- [Vite](https://vitejs.dev/)
- [Giphy API](https://developers.giphy.com/) *(para los GIFs)*

---

## 📦 Instalación

```bash
# Clona el repositorio
git clone https://github.com/Jorge-22f/chat-indecision-app.git

# Entra al proyecto
cd chat-indecision-app

# Instala dependencias
npm install

# Corre el servidor de desarrollo
npm run dev
```

---

## 🧪 ¿Cómo funciona?

1. El usuario escribe en la caja de texto, si finaliza con una incognita ?.
2. La app consulta una API externa que responde con "sí" o "no".
3. Se muestra la respuesta junto con un GIF relacionado.
4. El componente de mensajes se actualiza y hace scroll automático.

---

## 📚 Aprendizajes clave

- Uso de `defineProps` y `defineEmits` en `<script setup>`
- Manejo de reactividad con `ref`, `watch` y `computed`
- Buenas prácticas con TypeScript en Vue
- Modularización y separación de responsabilidades

---

## 🤝 Autor

**Jorge** – apasionado por el diseño de sistemas escalables, aprendiz técnico y explorador de buenas prácticas en desarrollo web.

---

## 📄 Licencia

Este proyecto es de uso educativo y libre. Puedes modificarlo, compartirlo y adaptarlo como desees.

---

¿Quieres que te ayude a agregar una sección de capturas, documentación técnica o incluso una guía para extender la app con respuestas más inteligentes? Podemos hacerlo juntos.
