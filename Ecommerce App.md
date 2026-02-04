🛒 SasmalStore | Full-Stack E-Commerce Platform

A robust MERN-stack e-commerce application featuring dynamic product management, advanced filtering, and secure user authentication.
This project is not just a storefront; 
it is a demonstration of solving real-world configuration and data integration challenges.

----

🔗 **Live Demo:**
- [Production Site](https://react-ecommerce-project-manaswini-sasmals-projects.vercel.app/)
- Backend API: Hosted on Render

---

## 🚀 Features

**Product Gallery**  
  Browse items with images, names, prices and quick “Add to Cart” buttons.

- **Search & Filter**  
  Find products by name or category.

- **Shopping Cart**  
  Add, update, or remove items. Cart state persists across sessions.

- **Checkout Flow**  
  Review order, enter shipping details, and simulate payment.

- Secure Checkout: Protected routes powered by Auth0 to ensure user data privacy.
- Dynamic Data: Products are fetched in real-time from a MongoDB collection.
  

---

## 🛠️ Tech Stack

* **React.js (v18)**
* **React Router DOM**
* **Axios**
* **Styled-Components**
* **React Icons**
* **JavaScript (ES6+)**
* **HTML5 & CSS3**
* Frontend: React.js, Styled Components, Context API
* Backend: Node.js, Express.js
* Database: MongoDB Atlas
* Auth: Auth0 (Secure Identity Management)

---

## 🔐 Authentication

* Authentication is handled using **Auth0**
* Supports:

  * User Login
  * User Logout
  * Protected routes

This provides a secure and real-world authentication flow.

---

## 🌐 Routing

Routing is implemented using **React Router DOM v6**, including:

* Home Page
* Product Listing Page
* Product Details Page
* Authentication Pages
* Fallback / Error Routes

----

## Challenges & Solutions

- Problem: Encountered "Oops! Something went wrong" errors during login after deployment.
- Diagnosis: Discovered that Auth0 is extremely strict with URI formatting; a single extra comma or missing URL in the "Allowed Callback URLs" prevents authentication.
- Solution: Meticulously synced the Vercel production link and localhost:3000 in the Auth0 dashboard, ensuring no trailing commas remained in the configuration.

1. Auth0 Configuration & Mismatched URIs







