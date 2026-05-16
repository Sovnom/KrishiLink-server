# KrishiLink Server - Agro-Social Network API (Server-Side)

This repository hosts the dedicated backend RESTful API for **KrishiLink**. It acts as the secure core handling data persistence, relational structure management for agro-posts, connection requests routing, and automated stock controls for the entire platform.

## 🔗 Live Deployment Links
- **Production Server URL:** [https://krishilink-server-blush.vercel.app](https://krishilink-server-blush.vercel.app)
- **Associated Live Client:** [https://krishilink-app.netlify.app](https://krishilink-app.netlify.app)

---

## 🌟 Core Backend Features

- **Relational Object-ID Interest Injection:** When an interest request is submitted, the backend dynamically generates a unique MongoDB `ObjectId` instance and injects it directly into the embedded `interests` array of the specific target crop document.
- **Atomic Stock Management Logic:** Built-in conditional transactional flows ensure that accepting a pending connection request automatically reduces the estimated stock quantity of the respective crop item in real time.
- **Secure CRUD API Routings:** Comprehensive endpoints crafted using Express.js to seamlessly parse query limits for the homepage (Latest 6 posts), execute regex-based text search parameters, and serve personalized datasets for private user dashboards.
- **Strict Owner-Matching Permissions:** Structural logic safeguards core endpoints ensuring that only authorized accounts matching the original listing owner block can run update or delete commands.
- **Optimized Environment Variable Masking:** Fully configures production variables for MongoDB Atlas credentials via secured hostings on Vercel, preventing unauthorized access to raw collections.

---

## 🛠️ Technologies & Packages Used

- **Runtime Environment:** Node.js
- **Framework:** Express.js
- **Database Server:** MongoDB Atlas
- **Security & Utilities:** dotenv, cors, mongodb

---

## 🚀 Local Installation Guide

Follow these steps to deploy and run the API server on your local machine:

1. **Clone the repository:**
   ```bash
   git clone [https://github.com/YOUR_GITHUB_USERNAME/krishilink-server.git](https://github.com/YOUR_GITHUB_USERNAME/krishilink-server.git)
   cd krishilink-server
