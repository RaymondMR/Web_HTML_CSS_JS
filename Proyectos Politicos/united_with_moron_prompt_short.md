
# 🧠 Project: Political Platform “United with Morón”

## 🎯 GOAL
Build a **modern, participatory site** for the **“United with Morón”** movement to support **Prof. Raúl Morón Orozco** as Governor of Michoacán (2027).  
It will inform, connect, and engage citizens with his proposals and actions.

---

## ⚙️ TECH STACK
- **Backend:** Laravel 12  
- **Frontend:** InertiaJS + ReactJS  
- **Styling:** Tailwind CSS  
- **Database:** PostgreSQL  
- **Auth:** Laravel Breeze / Jetstream  
- **Deployment:** Docker-ready  

---

## 🏠 MAIN SECTIONS

### 1️⃣ Home Page
Magazine-style with hero image, slogan:  
> “United with Morón — For a Fair and Forward-Thinking Michoacán.”  
Links: Biography, Proposals, Citizen Proposals, News, Chat, Login/Register.

### 2️⃣ Biography (`/biografia`)
Timeline + photo gallery + download biography (PDF).

### 3️⃣ Government Proposals (`/propuestas`)
Cards by topic (Education, Health, Economy, etc.). Each opens details with text/images/video.

### 4️⃣ Citizen Proposals (`/propuestas-ciudadanas`)
Form: title, description, category, name, email.  
Requires login. Users can comment or vote. Admin moderates.

### 5️⃣ News Blog (`/noticias`)
Cards with image, title, date, short text, and **Read more** link.  
Full post view with comments. Admin CRUD for posts.

### 6️⃣ Community Chat (`/chat`)
WhatsApp-style chat with channels: General, Regional, Admin.  
Real-time via Laravel Echo + Pusher/Socket.IO.

---

## 🔐 ROLES
- **Guest:** view only  
- **User:** comment, propose, chat  
- **Admin:** manage users, content  

---

## 🧩 ADMIN PANEL
At `/admin`: manage News, Proposals, Users, Comments.

---

## 🎨 DESIGN
- Colors: Red `#A01717`, Gold `#D4AF37`, Light Gray `#F3F4F6`  
- Fonts: Montserrat (titles), Inter (text)  
- Responsive + smooth Tailwind transitions.  
- Modern, institutional style.

---

## 🧠 FUTURE IDEAS
- Map of supporters  
- Polls / surveys  
- Newsletter  
- Stats dashboard  
- Social media links  

---

## 📦 STRUCTURE
```
/resources/js/Pages
  Home.jsx, Biografia.jsx, Propuestas.jsx, PropuestasCiudadanas.jsx, Noticias.jsx, Chat.jsx
  /Admin: Dashboard.jsx, NoticiasCrud.jsx, PropuestasCrud.jsx, UsuariosCrud.jsx

/resources/js/Components
  Navbar.jsx, Footer.jsx, NewsCard.jsx, ProposalCard.jsx, ChatBox.jsx
```

---

## 🧑‍💻 REQUIREMENTS
Generate:
- Base Laravel + Inertia + React + Tailwind app  
- Routes + main views above  
- Basic auth + PostgreSQL migrations  
- Clean, minimal, expandable design  

---

## 💬 TONE
> “Unity, hope, and commitment to Michoacán.”  
Inspire trust and civic participation.

---

## ✅ DELIVERABLES
1. Functional base app with navigation  
2. Auth (login/register/logout)  
3. CRUD for News & Proposals  
4. Basic chat  
5. Responsive UI  
6. README for setup  

---

## 🧭 NOTE
Keep modular architecture for future extensions (polls, dashboard, etc.).
I want yo to create a website with the project features specified above:
If you don't have a way to create it entirely in Laravel, at least create the frontend in React.
