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
* Formspree for contact page

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

1. Auth0 Configuration & Mismatched URIs

- Problem: Encountered "Oops! Something went wrong" errors during login after deployment.
- Diagnosis: Discovered that Auth0 is extremely strict with URI formatting; a single extra comma or missing URL in the "Allowed Callback URLs" prevents authentication.
- Solution: Meticulously synced the Vercel production link and localhost:3000 in the Auth0 dashboard, ensuring no trailing commas remained in the configuration.

2. Lessons Learned
- Environmental Parity: Learned how to manage different settings for Local vs. Production environments.
- Persistence: Developed a systematic approach to debugging third-party API errors by reading logs and documentation carefully.

3. The 60-Second "Cold Start" (Render & MongoDB)
- The Issue: After being inactive, the website would load, but the products wouldn't appear for about 60 seconds.
- The Diagnosis: I realized this is due to using Render's Free Tier for the backend. When the server is not in use, Render "spins it down" to save resources. When a new user visits, the server needs about a minute to "wake up" and re-establish a connection to MongoDB Atlas.
- The Solution: I documented this in the README to manage user expectations. In a professional environment, this would be solved by upgrading to a "Paid" instance for 100% uptime.

4. Vercel Deployment: "Treating Warnings as Errors"
- The Issue: My deployment failed with the error: Treating warnings as errors because process.env.CI = true.
- The Diagnosis: By default, many CI/CD platforms (like Vercel and GitHub Actions) treat simple linting warnings (like an unused variable) as fatal errors, stopping the build.
- The Solution: I solved this by modifying the Build Command in my Vercel settings. I changed npm run build to CI=false npm run build. This allowed the project to deploy successfully while I worked on cleaning up the warnings in the code.









