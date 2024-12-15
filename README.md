# Reservation Management System

## Description
The Reservation Management System is a full-stack web application for managing restaurant reservations. It provides features for user authentication, table reservation, and secure data communication through HTTPS. The application has a modular architecture for scalability and reliability.

## Features
- **User Authentication:** Secure registration and login using JWT.
- **Dynamic Reservation System:** Allows users to reserve tables by providing required details.
- **HTTPS Integration:** Ensures secure communication for all data transmissions.
- **Error Handling:** Robust feedback system for user input validation and runtime errors.
- **RESTful APIs:** Backend services built with scalability in mind.

## Technologies Used
- **Frontend:** React.js (running on port 5173)
- **Backend:** Node.js, Express.js (running on port 4000)
- **Database:** MongoDB
- **Authentication:** JSON Web Tokens (JWT)
- **Deployment:** Vercel

## Installation

### Prerequisites
- Node.js installed on your machine.
- MongoDB Atlas or a local MongoDB instance.

### Steps

#### Backend
1. Navigate to the backend directory:
   ```bash
   cd backend
   ```

2. Install backend dependencies:
   ```bash
   npm install
   ```

3. Configure environment variables by creating a `.env` file in the backend directory:
   ```
   MONGO_URI=<your_mongo_connection_string>
   JWT_SECRET=<your_jwt_secret>
   ```

4. Start the backend server:
   ```bash
   npm run dev
   ```
   The backend server will start on `http://localhost:4000`.

#### Frontend
1. Navigate to the frontend directory:
   ```bash
   cd frontend
   ```

2. Install frontend dependencies:
   ```bash
   npm install
   ```

3. Start the frontend:
   ```bash
   npm run dev
   ```
   The frontend will be available at `http://localhost:5173`.

---

## User Documentation

### For Users:
1. **Access the Website**:
   Open your browser and visit `http://localhost:5173`.

2. **Register a New Account**:
   - Click on the **Register** button on the homepage.
   - Provide your full name, email, and password.
   - Click **Submit** to create your account.

3. **Login**:
   - Click on the **Login** button.
   - Enter your registered email and password.
   - After successful login, you will be redirected to the home page.

4. **Make a Reservation**:
   - Navigate to the reservation form.
   - Fill in the required details:
     - First Name
     - Last Name
     - Email
     - Phone Number
     - Reservation Date and Time
   - Submit the form to create a reservation.
   - You will receive a confirmation message.

5. **Logout**:
   - Click the **Logout** button to end your session.

---

## Project Structure

### Backend
```
backend/
|-- controllers/
|   |-- reservation.js
|-- models/
|   |-- User.js
|   |-- Reservation.js
|-- middlewares/
|   |-- authMiddleware.js
|   |-- error.js
|-- routes/
|   |-- auth.js
|   |-- reservationRoute.js
|-- dbConnection.js
|-- server.js
```

### Frontend
```
frontend/
|-- src/
|   |-- components/
|   |-- pages/
|   |-- context/
|-- App.jsx
|-- index.html
```

---

## Usage
1. Visit `http://localhost:5173` to access the application.
2. Register as a new user or log in with existing credentials.
3. Fill out the reservation form and submit it to create a reservation.
4. Logout after completing your tasks.

---

## License
This project is licensed under the MIT License.
