# 🍽️ KindBite: Food Waste Management App
"Kindness tastes better when shared."

->KindBite is a web platform that connects food donors with those in need to reduce food waste and fight hunger.

->Donors can easily share food details, images, and location, while receivers can browse and collect nearby donations.

->Built with a clean UI and smart backend, KindBite makes food sharing fast, simple, and impactful.         



## 🚀 Features

### 👥 User & Admin Management

* ✅ **User Registration & Login** with JWT-based authentication
* 📧 **Email verification via Nodemailer** during registration
* 🔐 **Admin login** with protected credentials and dashboard access

### 🍱 Food Donation System

* 📝 **Donors can fill a form** with:

  * Name
  * Food title & description
  * Quantity
  * **Location** (On google maps)
  * Image of the food
* 🧾 **Submissions stored** in MongoDB for tracking and management

### 📍 Location Sharing

* 📌 **Donors can share their location** when donating food
* 📍 All **receivers can view the donor's location** along with food details
* 🗺️ Enables faster and more efficient pickup by nearby receivers

### ☁️ Image Upload Handling

* 📂 Images are **temporarily stored** using `multer`
* ☁️ Then uploaded to **Cloudinary** for permanent storage
* 🔗 Image URLs are saved in the database with each donation

### 🔍 Food Listing & Management

* 🗂️ **All food donations are listed** on the platform
* 🧹 **Admin can manage** food entries – approve, delete, or update
* 📦 Receivers can **browse food items** and see donor details

### 🌐 Frontend Integration

* ⚡ Built using **React + Vite**
* 🔄 Uses `VITE_BACKEND_URL` to connect with backend APIs
* 📱 Fully responsive and user-friendly interface



## 🔧 Tech Stack

| Layer      | Technology                |
|------------|---------------------------|
| Frontend   | React.js, Axios, CSS      |
| Backend    | Node.js, Express.js       |
| Database   | MongoDB with Mongoose     |
| Tools      | Multer (file uploads), dotenv, nodemailer,cloudinary |



## 🛠️ Installation Guide

### ✅ Prerequisites

- Node.js installed
- MongoDB running (local or cloud)
- npm (Node package manager)


## 🔙 Backend Setup

### 1. Navigate to backend

cd backend


### 2. Install dependencies

npm install


### 3. Create `.env` file

JWT_SECRET=your_jwt_secret_key

MONGODB_URL=your_mongodb_connection_string

GMAIL_USER=your_verified_email@gmail.com

GMAIL_PASS=your_gmail_app_password

ADMIN_EMAIL=admin_email@example.com

ADMIN_PASS=your_admin_password


### 4. Start server

npm run dev

Or with nodemon (auto-restarts on changes):

npm install -g nodemon
nodemon index.js


## 🔜 Frontend Setup

### 1. Navigate to frontend

cd frontend


### 2. Install dependencies

npm install


### 3. Create `.env` file

VITE_BACKEND_URL=your_backend_URL


### 4. Start React app

npm run dev
The app will run on `http://localhost:5173`.


## 5. Image Uploads
->Images are temporarily stored in the uploads/ folder using multer middleware.

->After that, the images are uploaded to Cloudinary, a cloud-based image hosting service, for permanent storage and access.


## 6. Login & Register Notes
Email Verification: While registering a new account, the user's email is verified using Nodemailer to ensure authenticity.


## 🧪 Sample Test Accounts

DONOR:
Email: Raj
Password: 12345

RECEIVER 1:
Username:Raghu
Password:123456

RECEIVER 2:
Username:Bhaskar
Password:12345

ADMIN:
Username:Rajnish
Password:Rajnish@2001



## ⚙️ Useful Scripts

| Action               | Command                |
|----------------------|------------------------|
| Start backend        | `node index.js`        |
| Start backend (dev)  | `nodemon index.js`     |
| Start frontend       | `npm start`            |
| Install backend deps | `npm install`          |
| Install frontend deps| `npm install`          |


## 📸 Screenshots

Homepage:https://res.cloudinary.com/dhjaboitg/image/upload/v1751715592/Screenshot_2025-07-05_170330_gmjgqa.png

AllDonations Page:https://res.cloudinary.com/dhjaboitg/image/upload/v1751715797/Screenshot_2025-07-05_171300_vu77t5.png

Review Page:https://res.cloudinary.com/dhjaboitg/image/upload/v1751715884/Screenshot_2025-07-05_171409_fecmc5.png

Donation Page:https://res.cloudinary.com/dhjaboitg/image/upload/v1751715960/Screenshot_2025-07-05_171544_blmtsn.png

Profile Page:https://res.cloudinary.com/dhjaboitg/image/upload/v1751716046/Screenshot_2025-07-05_171703_mhmmib.png


## 📬 Contact
For questions or feedback, feel free to contact the developer. 

