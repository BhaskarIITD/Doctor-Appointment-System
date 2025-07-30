for admin login, use 
email : admin@example.com
password : greatstack123


About the Project

This project is a robust and user-friendly Doctor Appointment Booking System designed to streamline the process of scheduling and managing medical appointments. It provides functionalities for both patients to book appointments and doctors to manage their schedules and patient information. The system aims to reduce administrative overhead, improve patient access to healthcare, and enhance the overall efficiency of clinics and individual practitioners.

Features
User Authentication & Authorization: Secure login and registration for patients and doctors with role-based access control.

Doctor Management:

Doctors can register and manage their profiles (specialty, experience, fees, availability).

Doctors can view and manage their booked appointments.

Patient Management:

Patients can search for doctors by specialty, name, or location.

Patients can view doctor profiles and their available slots.

Patients can book, view, and cancel appointments.

Patients receive confirmation and reminder notifications (if implemented).

Appointment Scheduling:

Real-time availability checking.

Conflict prevention for overlapping appointments.

Admin Panel (Optional/Future):

Manage users (patients, doctors).

Overview of system activity.

(Add if you have an admin panel)

Technologies Used
Backend:

Node.js

Express.js (Web Framework)

MongoDB (NoSQL Database)

Mongoose (MongoDB ODM)

JWT (JSON Web Tokens) for authentication

Bcrypt.js for password hashing

(Add any other libraries/technologies you used, e.g., Nodemailer for emails, Multer for file uploads)

Frontend (If applicable, specify framework/library):

React.js / Angular / Vue.js / HTML, CSS, JavaScript

(Add any specific UI libraries, e.g., Tailwind CSS, Bootstrap)

Getting Started
Follow these instructions to get a copy of the project up and running on your local machine for development and testing purposes.

Prerequisites
Before you begin, ensure you have the following installed:

Node.js (LTS version recommended)

npm (Node Package Manager, comes with Node.js) or Yarn

MongoDB (running locally or accessible via a cloud service like MongoDB Atlas)

Git

Installation
Clone the repository:

git clone https://github.com/your-username/doctor-appointment-system.git
cd doctor-appointment-system

Install backend dependencies:

cd backend # Or whatever your backend folder is named
npm install # or yarn install

Install frontend dependencies (if applicable):

cd ../frontend # Or whatever your frontend folder is named
npm install # or yarn install

Environment Variables
Create a .env file in your backend directory (or the root of your project if it's a single folder) and add the following environment variables:

PORT=5000
MONGO_URI=mongodb://localhost:27017/doctor_appointments # Or your MongoDB Atlas URI
JWT_SECRET=your_jwt_secret_key_here # Use a strong, random string
JWT_LIFETIME=1d # e.g., 1h, 1d, 30d
# Add any other environment variables your application uses (e.g., for email services, cloud storage)

Running the Application
Start the MongoDB server (if running locally).

Start the backend server:

cd backend
npm start # or node server.js or node index.js depending on your entry file

The backend server should now be running on http://localhost:5000 (or your specified PORT).

Start the frontend development server:

cd frontend
npm start

The frontend application should open in your browser, typically at http://localhost:3000.

Folder Structure
.
├── backend/
│   ├── config/              # Database connection, JWT config, Cloudinary config
│   ├── controllers/         # Handles request logic (e.g., authController.js, doctorController.js)
│   ├── models/              # Mongoose schemas (e.g., User.js, Doctor.js, Appointment.js)
│   ├── routes/              # API routes (e.g., authRoutes.js, doctorRoutes.js)
│   ├── middleware/          # Authentication middleware, error handling
│   ├── utils/               # Utility functions (e.g., password hashing)
│   ├── server.js            # Main application entry point
│   └── package.json
├── frontend/
│   ├── public/
│   ├── src/
│   │   ├── components/
│   │   ├── pages/
│   │   ├── services/
│   │   └── App.js
│   └── package.json
├── .env          
├── .gitignore

Contact
Bhaskar Roy - ce1221046@iitd.ac.in
Project Link: https://github.com/BhaskarIITD/Doctor-Appointment-System
