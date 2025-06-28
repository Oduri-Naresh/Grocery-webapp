# Grocery-webapp
**GROCERY WEB APP - MERN STACK APPLICATION**

---

### 1. INTRODUCTION

#### 1.1 Project Overview

The Grocery Web App is a comprehensive, user-friendly web-based platform designed to simplify the grocery shopping process. It eliminates the traditional inefficiencies of in-store shopping—such as long queues, inventory confusion, and limited access—by offering a smooth, digital grocery experience for users and administrators alike.

Built using the MERN stack (MongoDB, Express.js, React.js, Node.js), the application allows users to register, browse grocery items with filters, manage their carts, securely complete purchases, and track their deliveries. Admins can manage inventory, monitor orders, and oversee customer accounts.

#### 1.2 Purpose

The primary purpose of the Grocery Web App is to:

* Provide a digital-first grocery shopping platform.
* Enable real-time inventory access and secure checkout.
* Allow administrators to manage backend operations seamlessly.
* Reduce operational friction and enhance user convenience.

---

### 2. IDEATION PHASE

#### 2.1 Problem Statement

In a busy world, customers face difficulty in finding time for traditional grocery shopping. Limited store hours, long queues, and lack of access to a full product range often lead to frustration. For administrators, managing inventory manually is inefficient.

The Grocery Web App addresses these issues by providing:

* Real-time product listing and filtering.
* A secure and user-friendly shopping and checkout process.
* Delivery scheduling and tracking.
* Centralized admin control of products and orders.

#### 2.2 Empathy Map Canvas

| THINKS                                    | FEELS                              | SAYS                                   | DOES                 |
| ----------------------------------------- | ---------------------------------- | -------------------------------------- | -------------------- |
| “I want to find fresh groceries quickly.” | Frustrated with long queues        | “I wish I could get it all delivered.” | Shops late at night  |
| “Can I filter by dietary needs?”          | Relieved after successful delivery | “This should be easier.”               | Tracks orders online |

---

### 3. REQUIREMENT ANALYSIS

#### 3.1 Customer Journey Map

| Stage           | User Action                         | Emotion   | Touchpoints             | Opportunities for Improvement |
| --------------- | ----------------------------------- | --------- | ----------------------- | ----------------------------- |
| Awareness       | Searches for an online grocery site | Curious   | Social media, Google    | SEO, clean landing page       |
| Registration    | Creates account                     | Hopeful   | Sign-up form            | Streamlined onboarding        |
| Browsing        | Filters and selects products        | Confident | Product dashboard       | Personalized recommendations  |
| Cart & Checkout | Adds items and pays                 | Relieved  | Cart page, payment form | One-click checkout, wallet    |
| Confirmation    | Order confirmation                  | Reassured | Email/SMS               | Instant updates               |
| Delivery        | Receives groceries                  | Satisfied | Delivery dashboard      | Real-time tracking            |

#### 3.2 Functional Requirements

* User Authentication
* Product Search & Filtering
* Shopping Cart
* Order Placement & Tracking
* Admin Dashboard Management

#### 3.3 Non-Functional Requirements

* Scalability
* Responsive Design
* Fast Performance
* Secure Authentication

---

### 4. SOLUTION DESIGN

#### 4.1 Proposed Solution

To solve the core issues in grocery shopping, the application provides:

* Real-time grocery inventory.
* Easy product discovery through filters.
* A fast and intuitive checkout process.
* Real-time order tracking.
* Admin features for inventory and order management.

#### 4.2 Solution Architecture

* **Frontend**: React.js (Bootstrap, Material UI, Axios)
* **Backend**: Node.js + Express.js
* **Database**: MongoDB (Mongoose ODM)
* **Authentication**: JWT + bcrypt
* **Hosting**: Vercel (Frontend), Render (Backend), MongoDB Atlas (Database)

---

### 5. DATABASE DESIGN

#### Mongoose Schemas

```js
const userSchema = new mongoose.Schema({ firstname, lastname, username, email, password });
const categorySchema = new mongoose.Schema({ category, description });
const productSchema = new mongoose.Schema({ productname, description, price, image, category, countInStock, rating, dateCreated });
const cartSchema = new mongoose.Schema({ userId, productId, quantity });
const orderSchema = new mongoose.Schema({ firstname, lastname, user, phone, productId, productName, quantity, price, status, paymentMethod, address, createdAt });
```

---

### 6. FRONTEND DESIGN

#### Pages Implemented

* Landing Page
* User Registration/Login
* Product Dashboard
* Cart Page
* Checkout Page
* Order Tracking Page
* Admin Panel (Products & Orders)

#### UI Technologies Used

* React.js (JSX Components)
* Bootstrap 5 & Material UI
* Axios (API integration)
* React Router DOM

---

### 7. FUNCTIONAL AND PERFORMANCE TESTING

#### 7.1 Testing Scenarios

| Test Scenario | Description                       | Expected Result       |
| ------------- | --------------------------------- | --------------------- |
| API Load      | 100 users checkout simultaneously | < 2 sec response time |
| Cart Load     | 1000 items added/removed          | No crash              |
| DB Load       | 10,000+ entries queried           | < 1.5 sec             |
| Auth Load     | Multiple logins/signups           | Secure, stable        |
| Image Upload  | Product images added              | < 3 sec load          |

#### 7.2 Tools Used

* Postman (API Testing)
* Chrome DevTools (Frontend Load)
* MongoDB Atlas Dashboard
* Apache JMeter (Stress Testing)

---

### 8. RESULTS

* All critical features tested successfully.
* Responsive UI across devices.
* Backend supported high concurrency.
* Admin functionality performed well under load.
* Secure authentication flow validated.

---

### 9. FUTURE SCOPE

* Online payment integration (Razorpay, Stripe).
* Native mobile application (Flutter).
* Product recommendation engine (AI/ML).
* Multilingual support (i18n).
* Role-based analytics for admin insights.

---

### 10. APPENDIX

* **Source Code**: [Google Drive Folder](https://drive.google.com/drive/folders/1RP-29p9mf-bbLAK5r7S4HSF_Itai0i1G?usp=drive_link)
* **Demo Video**: [Grocery Web App Demo](https://drive.google.com/file/d/1HLowcIqs2d8lxTprS2jqPmR4AOnUW8xD/view?usp=drive_link)

---

**Thank you for exploring our Grocery Web App!**
