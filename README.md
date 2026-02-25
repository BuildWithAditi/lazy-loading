# 📊 React Dashboard with Routing & Lazy Loading

A modern and responsive React Dashboard application built using **Vite**.  
This project demonstrates dynamic routing, lazy loading (code splitting), and a clean modular layout.

---

## 🚀 Features

- 🧭 React Router v6
- ⚡ Lazy Loading using `React.lazy()`
- ⏳ Suspense with custom Loader
- 📂 Modular folder structure
- 🎨 Clean sidebar layout
- 📱 Responsive-ready structure

---

## 🛠 Tech Stack

- React
- Vite
- React Router DOM
- CSS

---

## 📁 Project Structure

```
react-app/
│
├── src/
│   ├── layout/
│   │   ├── Sidebar.jsx
│   │   └── Navbar.jsx
│   │
│   ├── pages/
│   │   ├── Home.jsx
│   │   ├── Analytics.jsx
│   │   ├── Orders.jsx
│   │   ├── Users.jsx
│   │   └── Settings.jsx
│   │
│   ├── components/
│   │   └── Loader.jsx
│   │
│   ├── App.jsx
│   ├── App.css
│   ├── main.jsx
│   └── index.css
│
├── index.html
├── package.json
└── vite.config.js
```

---

## ⚡ Lazy Loading Implementation

Each route is dynamically imported:

```js
const Home = lazy(() => import("./pages/Home"));
```

Wrapped inside:

```jsx
<Suspense fallback={<Loader />}>
```

This improves performance by loading components only when required.

---

## 🧭 Available Routes

- `/` → Home  
- `/analytics` → Analytics  
- `/orders` → Orders  
- `/users` → Users  
- `/settings` → Settings

---📷 Screenshots
<img width="1914" height="933" alt="Screenshot 2026-02-17 120315" src="https://github.com/user-attachments/assets/253402e3-3b32-41dd-81b0-e3e784073952" />
<img width="1918" height="871" alt="Screenshot 2026-02-17 120229" src="https://github.com/user-attachments/assets/f4471bd7-ad98-4780-9bfb-5782f7402209" />
<img width="1904" height="892" alt="Screenshot 2026-02-17 120245" src="https://github.com/user-attachments/assets/33fdefa3-47da-421a-b504-b36b0a8fbbec" />

---

## 🛠 Installation & Setup

### 1️⃣ Clone the Repository

```bash
git clone https://github.com/yourusername/react-dashboard.git
```

### 2️⃣ Navigate to Project Folder

```bash
cd react-dashboard
```

### 3️⃣ Install Dependencies

```bash
npm install
```

### 4️⃣ Run Development Server

```bash
npm run dev
```

Open in browser:

```
http://localhost:5173
```

---

## 📦 Dependencies

- react
- react-dom
- react-router-dom
- vite

---

## 🎯 Learning Outcomes

- React functional components
- React Router v6
- Lazy loading & Suspense
- Modular project architecture
- Clean dashboard layout design

---
