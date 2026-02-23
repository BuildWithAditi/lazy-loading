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

## 🚀 Future Improvements

- Active route highlighting
- Dark mode toggle
- Protected routes
- Redux integration
- API integration

---

## 👩‍💻 Author

**Aditi Parmar**  
B.E CSE (AI & ML)  
Chandigarh University  

---

⭐ If you found this project helpful, consider giving it a star!
