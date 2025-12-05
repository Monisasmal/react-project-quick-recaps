# ✅ Blog App — Project

A blog application built with React + Firebase where users can navigate between pages and manage blog content.

## 🧩 Tech Stack Used

- React 18
- React Router DOM 7 → For page navigation
- Firebase → For backend services (Auth, Firestore, or Storage)
- Vite → Build tool & dev server
- JavaScript (ES6+), React Hooks, Custom CSS

## 🔧 Key Features

- User authentication (Firebase Auth)
- Protected routes for authenticated users (React Router)
- Real-time updates (Firestore live sync)
- Custom CSS styling
- Responsive layout

## 🎯 Why I Used These Technologies
- React → Easy to structure UI and manage components
- Firebase → Fast backend without server setup
- React Router → Smooth navigation between pages
- Vite → Extremely fast development server
- Custom CSS → Full styling control, no dependency on frameworks

## 🛠️ Challenges
Challenge 1: Handling auth + route protection
Solution: Used Firebase Auth state listener + React Router <ProtectedRoute> wrapper
Challenge 2: Managing realtime data from Firestore
Solution: Used Firestore onSnapshot() to auto-update UI without refresh
Challenge 3: App structure became messy
Solution: Split code into reusable components & organized pages folder


