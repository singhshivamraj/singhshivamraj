<p align="center">
  <img src="./hero.svg?v=2" alt="Shivam Raj — Full Stack Developer | MERN | Java & DSA" width="760" />
</p>

<p align="center">
  <a href="https://www.linkedin.com/in/shivam-rajfullstack">
    <img src="https://img.shields.io/badge/LinkedIn-Connect-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" />
  </a>
  <a href="mailto:shivamraj6436@gmail.com">
    <img src="https://img.shields.io/badge/Email-Let's%20Talk-D14836?style=for-the-badge&logo=gmail&logoColor=white" />
  </a>
  <img src="https://img.shields.io/badge/Open%20to-SDE%20%7C%20Full%20Stack-111827?style=for-the-badge" />
</p>

<br>

## About

I'm **Shivam Raj**, a B.Tech Computer Science student at **Subharti University**, focused on building production-ready full-stack applications with the **MERN stack**.

I enjoy taking an idea from **database schema → backend APIs → frontend → deployment** and making it work as a real product.

Currently, I'm:
- Building full-stack applications with **React, Node.js, Express and MongoDB**
- Solving **DSA problems in Java**
- Exploring real-world backend concepts like **authentication, payments, APIs and deployment**
- Building projects that are actually **deployed and usable**

**Looking for:** Software Developer / SDE / Full Stack opportunities  
**Internships:** Available now  
**Full-time:** Available from 2027

---

## 🚀 Featured Projects

### 🛍️ GenZVibe — Full Stack E-commerce

A production-style MERN e-commerce platform with a complete shopping and payment workflow.

**Built with:** React · Node.js · Express · MongoDB · Razorpay · Cloudinary

**Highlights**
- User authentication and protected routes
- Product browsing, cart and checkout
- Razorpay payment integration
- **Backend payment signature verification**
- Orders created only after successful verification
- Admin dashboard with sales analytics
- Product and order management
- Image uploads through Cloudinary
- Deployed full-stack application

**Live:** [genzvibe.onrender.com](https://genzvibe.onrender.com)  
**Source:** [GitHub Repository](https://github.com/singhshivamraj/GenZVibe)

---

### 🏠 Nestio — Hotel & Property Booking

An Airbnb/OYO-style property booking platform focused on authentication, listings, reviews and location-based discovery.

**Built with:** Node.js · Express · MongoDB · EJS · Passport.js · Joi · MapLibre

**Highlights**
- User authentication with Passport.js
- Create, edit and delete property listings
- Reviews and ratings
- Joi-based server-side validation
- Interactive map for property locations
- Search and category-based filtering
- Cloudinary image uploads
- Session-based authentication
- Deployed application

**Live:** [nestio-1.onrender.com](https://nestio-1.onrender.com/listings)  
**Source:** [GitHub Repository](NESTIO_REPO_LINK)

---

### 👨‍💻 DevCollab — Real-Time Coding Platform

**Currently building**

A collaborative coding platform where developers can create rooms and code together in real time.

**Planned stack:** React · Node.js · Socket.IO · Monaco Editor

**Core idea**
- Real-time collaborative coding
- Shared coding rooms
- Live code synchronization
- Multiple users in the same workspace
- Developer-focused collaboration features

**Source:** [GitHub Repository](DEVCOLLAB_REPO_LINK)

---

## 💳 Engineering Spotlight — Payment Verification

One part I'm particularly proud of in **GenZVibe** is how payment confirmation is handled.

The frontend never directly decides whether an order is paid.

```mermaid
flowchart LR
    A[Customer] --> B[Razorpay Checkout]
    B --> C[Payment Response]
    C --> D[Backend API]
    D --> E{Verify Signature}
    E -->|Valid| F[Create Order]
    E -->|Invalid| G[Reject Request]
    F --> H[(MongoDB)]
