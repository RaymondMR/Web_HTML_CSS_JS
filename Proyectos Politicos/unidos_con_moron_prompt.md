
# 🧠 Proyecto: Plataforma Política “Unidos con Morón”

## 🎯 OBJETIVO GENERAL
Crear una **plataforma digital integral** para el movimiento político **“Unidos con Morón”**, que impulse y promueva la candidatura del **Profesor Raúl Morón Orozco** a la Gubernatura del Estado de Michoacán (México) en las elecciones de 2027.

El sitio debe ser **dinámico, moderno y participativo**, permitiendo que simpatizantes y ciudadanos puedan:
- Informarse sobre la trayectoria del Profesor Raúl Morón Orozco.  
- Consultar sus propuestas políticas.  
- Enviar sus propias propuestas.  
- Interactuar mediante comentarios y chat en línea.  
- Acceder a contenido actualizado (noticias, comunicados, etc.).  

---

## ⚙️ TECNOLOGÍAS A UTILIZAR
- **Backend:** Laravel 12  
- **Frontend:** InertiaJS + ReactJS  
- **Estilos:** Tailwind CSS  
- **Base de datos:** PostgreSQL  
- **Autenticación:** Laravel Breeze o Jetstream (Inertia + React)  
- **Despliegue:** Listo para Docker o DigitalOcean  

---

## 🏠 SECCIONES PRINCIPALES

### 1️⃣ Home Page (Portada)
- Diseño tipo **revista política o campaña**, con imagen hero del Profesor Raúl Morón Orozco.
- Eslogan o frase central:  
  > “Unidos con Morón — Por un Michoacán Justo y con Futuro”.
- Contendrá botones de navegación:
  - **Biografía** (→ `/biografia`)
  - **Propuestas de Gobierno** (→ `/propuestas`)
  - **Propuestas Ciudadanas** (→ `/propuestas-ciudadanas`)
  - **Noticias y Comunicados** (→ `/noticias`)
  - **Chat Comunitario** (→ `/chat`)
  - **Registro / Login / Logout`)

---

### 2️⃣ Página: Biografía y Trayectoria (`/biografia`)
- Mostrar línea del tiempo (timeline) interactiva de la carrera del Profesor Morón.
- Incluir galería de fotos históricas y de eventos recientes.
- Botón para descargar biografía en PDF.

---

### 3️⃣ Página: Propuestas de Gobierno (`/propuestas`)
- Mostrar en tarjetas (cards) las principales propuestas.
- Cada tarjeta abre una vista detallada con texto, imágenes o video.
- Filtro por categoría: Educación, Salud, Economía, Campo, etc.

---

### 4️⃣ Página: Propuestas Ciudadanas (`/propuestas-ciudadanas`)
- Formulario para enviar propuestas o ideas:
  - Campos: Título, Descripción, Categoría, Nombre, Correo (opcional).
  - Requiere autenticación.
- Listado público de propuestas (con moderación por admin).
- Los usuarios pueden **votar o comentar** las propuestas.

---

### 5️⃣ Blog de Noticias (`/noticias`)
- Tarjetas con:
  - Imagen destacada  
  - Título  
  - Fecha  
  - Extracto del contenido  
  - Botón **“Leer más”**
- Página individual de noticia con sistema de **comentarios** (usuarios registrados).
- Panel de administración para agregar, editar y eliminar noticias.

---

### 6️⃣ Chat Comunitario (`/chat`)
- Espacio tipo WhatsApp/Telegram para miembros registrados.
- Canales:
  - General (todos los usuarios)
  - Equipos Regionales (por municipio)
  - Administración interna
- Notificaciones en tiempo real con **Laravel Echo + Pusher o Socket.IO**.

---

## 🔐 AUTENTICACIÓN Y ROLES
- **Usuario invitado:** solo puede leer noticias y biografía.
- **Usuario registrado:** puede comentar, chatear y enviar propuestas.
- **Administrador:** gestiona usuarios, noticias, propuestas y modera contenido.

---

## 🧩 PANEL ADMINISTRATIVO
Ruta: `/admin`
- Gestión de noticias (CRUD)
- Gestión de propuestas ciudadanas
- Moderación de comentarios y chat
- Gestión básica de usuarios (bloquear, asignar roles)

---

## 🎨 DISEÑO Y ESTILO
- Estilo sobrio, institucional y moderno.
- Colores base:
  - Rojo oscuro (`#A01717`)
  - Dorado (`#D4AF37`)
  - Gris claro (`#F3F4F6`)
- Tipografía recomendada:
  - **Titulares:** Montserrat
  - **Texto general:** Inter
- Diseño **responsive** (desktop / móvil).
- Animaciones suaves con Framer Motion o Tailwind Transitions.

---

## 🧠 FUNCIONES ADICIONALES FUTURAS
1. **Mapa interactivo de simpatizantes** (usuarios registrados por municipio).  
2. **Sistema de encuestas** (opinión sobre temas o propuestas).  
3. **Boletín informativo** con suscripción por correo electrónico.  
4. **Panel de estadísticas** (visitas, usuarios activos, interacciones).  
5. **Integración con redes sociales oficiales.**

---

## 📦 ESTRUCTURA DE CARPETAS (SUGERIDA)
```
/resources/js/Pages
    Home.jsx
    Biografia.jsx
    Propuestas.jsx
    PropuestasCiudadanas.jsx
    Noticias.jsx
    Chat.jsx
    Admin/
        Dashboard.jsx
        NoticiasCrud.jsx
        PropuestasCrud.jsx
        UsuariosCrud.jsx

/resources/js/Components
    Navbar.jsx
    Footer.jsx
    NewsCard.jsx
    ProposalCard.jsx
    ChatBox.jsx

/database/migrations
/routes/web.php
```

---

## 🧑‍💻 REQUISITOS DEL PROMPT
Quiero que generes:
- Toda la estructura inicial del proyecto Laravel con Inertia + React + Tailwind.  
- Las rutas y vistas principales mencionadas.  
- Un diseño inicial limpio, profesional y funcional.  
- Sistema de autenticación básico.  
- Estructura de base de datos en PostgreSQL (migraciones).  

---

## 💬 TONO Y MENSAJE POLÍTICO
El sitio debe transmitir:
> “Unidad, esperanza, experiencia y compromiso con Michoacán.”

Inspirar confianza, participación ciudadana y sentido de pertenencia.

---

## ✅ ENTREGABLES ESPERADOS
1. Proyecto base funcional (con navegación entre secciones).  
2. Sistema de autenticación (login, registro, logout).  
3. CRUDs para Noticias y Propuestas Ciudadanas.  
4. Chat básico funcional.  
5. Diseño responsive completo con Tailwind.  
6. README con instrucciones de instalación y ejecución.

---

## 🧭 NOTA FINAL
El proyecto debe poder ampliarse fácilmente en el futuro, con módulos adicionales (encuestas, mapas, dashboards), manteniendo una arquitectura limpia y escalable.
