## Doctor Appointment App ️

This is a full-stack web application built with the MERN stack (MongoDB, Express.js, React.js, and Node.js) that allows users to manage their doctor appointments.

### Features

* **User Management:**
    * Users can register for an account.
    * Users can log in to the system.
    * Users can apply to become doctors.
    * Admins must approve user applications to become doctors.
* **Appointment Management:**
    * Users can schedule appointments with approved doctors.
    * Doctors receive notifications about pending appointments.
    * Users receive notifications about appointment confirmations or cancellations.
* **Notification System:**
    * Admins are notified of new doctor applications.
    * Users receive notifications about the status of their doctor application.
    * Users receive notifications about appointment confirmations or cancellations.

### Technologies Used

**Frontend:**
* React / React with TypeScript (Optional)
* Redux Toolkit (State Management)
* Material UI (Components)
* Formik (Form Handling)
* RTK Query (API Data Fetching)

**Backend:**
* Node.js
* Express.js (Framework)

**Database:**
* MongoDB

### Screenshots

[Screenshots showcasing various functionalities of the app can be placed here. Consider using a service like Imgur for image hosting.]

### Setting Up the Environment

1. Create a `.env` file in your project root directory.
2. Add the following environment variables to your `.env` file:

**Backend:**

```
NODE_ENV=development
PORT=5000
DATABASE=YOUR_MONGODB_CONNECTION_STRING
```

**Frontend:**

```
REACT_APP_API_URL=http://localhost:5000/api/v1/
```

**Note:** Replace `YOUR_MONGODB_CONNECTION_STRING` with your actual MongoDB connection string.

### API Reference

#### Routes

All API endpoints are prefixed with `http://localhost:5000/api/v1/`.

**Users API**

* **Signup:**
    * Method: `POST`
    * Endpoint: `/signup`
* **Login:**
    * Method: `POST`
    * Endpoint: `/login`
* **Get All Users (Admin Only):**
    * Method: `GET`
    * Endpoint: `/`
* **Get User:**
    * Method: `GET`
    * Endpoint: `/:id`
* **Delete User (Admin Only):**
    * Method: `DELETE`
    * Endpoint: `/:id`
* **Verify User:**
    * Method: `GET`
    * Endpoint: `/verify-user/:id`
* **Book Appointment:**
    * Method: `POST`
    * Endpoint: `/book-appointment`
* **User Appointments:**
    * Method: `GET`
    * Endpoint: `/user-appointments/:id`
* **Mark All Notifications as Seen:**
    * Method: `POST`
    * Endpoint: `/mark-all-notification-as-seen`
* **Delete All Notifications:**
    * Method: `POST`
    * Endpoint: `/delete-all-notifications`
* **Change Doctor Status (Admin Only):**
    * Method: `POST`
    * Endpoint: `/change-doctor-status`

**Doctors API**

* **Get All Doctors:**
    * Method: `GET`
    * Endpoint: `/`
* **Get All Approved Doctors:**
    * Method: `GET`
    * Endpoint: `/approved-doctors`
* **Doctor Signup:**
    * Method: `POST`
    * Endpoint: `/signup`
* **Get Doctor:**
    * Method: `GET`
    * Endpoint: `/:id`
* **Update Doctor:**
    * Method: `PUT`
    * Endpoint: `/:id`
* **Get All Doctor Appointments:**
    * Method: `GET`
    * Endpoint: `/appointments/:id`
* **Get Booked Doctor Appointments:**
    * Method: `GET`
    * Endpoint: `/booked-appointments/:id`
* **Change Appointment Status:**
    * Method: `POST`
    * Endpoint: `/change-appointment-status`
* **Check Booking Availability:**
    * Method: `POST`
    * Endpoint: `/check-booking-availability`

