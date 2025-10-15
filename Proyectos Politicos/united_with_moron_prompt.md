
# 🧠 Project: Political Platform “United with Morón”

## 🎯 GENERAL OBJECTIVE
Create a **comprehensive digital platform** for the political movement **“United with Morón”**, which supports and promotes the candidacy of **Professor Raúl Morón Orozco** for Governor of the State of Michoacán (Mexico) in the 2027 elections.

The site must be **dynamic, modern, and participatory**, allowing supporters and citizens to:
- Learn about the background and career of Professor Raúl Morón Orozco.  
- Review his political proposals.  
- Submit their own proposals.  
- Interact through comments and live chat.  
- Access updated content (news, press releases, etc.).  

---

## ⚙️ TECHNOLOGIES TO USE
- **Backend:** Laravel 12  
- **Frontend:** InertiaJS + ReactJS  
- **Styling:** Tailwind CSS  
- **Database:** PostgreSQL  
- **Authentication:** Laravel Breeze or Jetstream (Inertia + React)  
- **Deployment:** Ready for Docker or DigitalOcean  

---

## 🏠 MAIN SECTIONS

### 1️⃣ Home Page (Landing Page)
- **Magazine-style design**, with a hero image of Professor Raúl Morón Orozco.
- Central slogan:  
  > “United with Morón — For a Fair and Forward-Thinking Michoacán.”
- Navigation buttons:
  - **Biography** (→ `/biografia`)
  - **Government Proposals** (→ `/propuestas`)
  - **Citizen Proposals** (→ `/propuestas-ciudadanas`)
  - **News & Announcements** (→ `/noticias`)
  - **Community Chat** (→ `/chat`)
  - **Register / Login / Logout**

---

### 2️⃣ Page: Biography and Career (`/biografia`)
- Display an interactive **timeline** of Professor Morón’s political and professional path.  
- Include a photo gallery (historic and recent events).  
- Button to download biography as PDF.

---

### 3️⃣ Page: Government Proposals (`/propuestas`)
- Display main proposals in **cards**.  
- Each card opens a detailed view with text, images, or videos.  
- Filter by category: Education, Health, Economy, Agriculture, etc.

---

### 4️⃣ Page: Citizen Proposals (`/propuestas-ciudadanas`)
- Form to submit ideas or proposals:
  - Fields: Title, Description, Category, Name, Email (optional).  
  - Requires authentication.  
- Public list of proposals (with admin moderation).  
- Users can **vote or comment** on proposals.

---

### 5️⃣ News Blog (`/noticias`)
- Cards containing:
  - Featured image  
  - Title  
  - Date  
  - Summary text  
  - Button **“Read more”**
- Individual news page with **comments system** (for registered users).  
- Admin panel to add, edit, and delete posts.

---

### 6️⃣ Community Chat (`/chat`)
- WhatsApp/Telegram-style chat space for registered members.  
- Channels:
  - General (all users)  
  - Regional Teams (by municipality)  
  - Internal Administration  
- Real-time notifications using **Laravel Echo + Pusher or Socket.IO**.

---

## 🔐 AUTHENTICATION AND ROLES
- **Guest:** can only read news and biography.  
- **Registered User:** can comment, chat, and submit proposals.  
- **Administrator:** manages users, news, proposals, and content moderation.

---

## 🧩 ADMIN PANEL
Route: `/admin`
- Manage news (CRUD)  
- Manage citizen proposals  
- Moderate comments and chat  
- Basic user management (block, assign roles)

---

## 🎨 DESIGN AND STYLE
- Elegant, institutional, and modern look.  
- Color palette:
  - Dark Red (`#A01717`)  
  - Gold (`#D4AF37`)  
  - Light Gray (`#F3F4F6`)  
- Recommended fonts:
  - **Headings:** Montserrat  
  - **Body text:** Inter  
- Fully **responsive design** (desktop and mobile).  
- Smooth animations via Framer Motion or Tailwind Transitions.

---

## 🧠 FUTURE ADD-ON FEATURES
1. **Interactive supporter map** (registered users by municipality).  
2. **Survey system** (opinions on topics or proposals).  
3. **Newsletter subscription** (email updates).  
4. **Statistics dashboard** (visits, active users, engagement).  
5. **Integration with official social media.**

---

## 📦 SUGGESTED FOLDER STRUCTURE
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

## 🧑‍💻 PROMPT REQUIREMENTS
Generate:
- Full project skeleton (Laravel + Inertia + React + Tailwind).  
- All main routes and views described.  
- A clean, professional, and functional design.  
- Basic authentication system.  
- PostgreSQL database structure (migrations).  

---

## 💬 POLITICAL TONE AND MESSAGE
The website must convey:
> “Unity, hope, experience, and commitment to Michoacán.”

Inspire trust, civic participation, and a sense of belonging.

---

## ✅ EXPECTED DELIVERABLES
1. Functional base project (with navigation).  
2. Authentication system (login, register, logout).  
3. CRUD for News and Citizen Proposals.  
4. Functional basic chat.  
5. Fully responsive Tailwind design.  
6. README with setup instructions.

---

## 🧭 FINAL NOTE
The project must be easily scalable in the future, with additional modules (polls, maps, dashboards), maintaining a clean and modular architecture.
