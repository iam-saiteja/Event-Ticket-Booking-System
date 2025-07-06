# Event Ticket Booking System

## Overview

This is a comprehensive event ticket booking system, built as a Firebase project. It handles user authentication, event management, ticket booking, and payment processing. The system is designed to be scalable and provides both administrative and user interfaces.

## Features

*   **User Authentication:** Secure user registration and login.
*   **Event Management:** Create, update, and manage various events.
*   **Ticket Booking:** Seamless process for users to book tickets for events.
*   **Payment Integration:** Handles payment processing for ticket purchases.
*   **Admin Dashboard:** Dedicated interface for administrators to manage events, users, and bookings.
*   **QR Code Generation:** For tickets or event entry.
*   **Email Notifications:** For booking confirmations and other updates.
*   **PDF Ticket Generation:** Generate printable tickets in PDF format.

## Technologies Used

*   **Backend:** Node.js, Express.js, Firebase Functions
*   **Database:** Firebase Firestore, Firebase Realtime Database
*   **Authentication:** Firebase Authentication, `bcryptjs` for password hashing, `jsonwebtoken` for token management.
*   **Storage:** Firebase Storage
*   **Hosting:** Firebase Hosting
*   **Frontend:** HTML, CSS (with Tailwind CSS), JavaScript
*   **Utilities:** `cors`, `moment` (for date/time handling), `multer` (for file uploads), `nodemailer` (for email), `pdf-lib` (for PDF generation), `qrcode` (for QR codes), `uuid` (for unique IDs).

## Getting Started

### Prerequisites

*   Node.js installed
*   Firebase CLI installed (`npm install -g firebase-tools`)
*   A Firebase project set up and linked to your local environment.

### Installation

1.  Clone the repository:
    ```bash
    git clone https://github.com/iam-saiteja/Event-Ticket-Booking-System.git
    ```
2.  Navigate to the project directory:
    ```bash
    cd Event-Ticket-Booking-System
    ```
3.  Install root dependencies:
    ```bash
    npm install
    ```
4.  Navigate to the `functions` directory and install its dependencies:
    ```bash
    cd functions
    npm install
    cd ..
    ```
5.  Link your Firebase project:
    ```bash
    firebase use --add
    ```
    (Follow the prompts to select your Firebase project.)

### Running Locally

To run the project locally using Firebase emulators:

```bash
firebase emulators:start
```

This will start emulators for Firestore, Functions, Hosting, and other services. The hosting URL will be provided in the terminal (usually `http://localhost:5000`).

### Deployment

To deploy the project to Firebase:

```bash
firebase deploy
```

This will deploy your Firebase Functions, Hosting, Firestore rules, and Storage rules.

## Project Structure

```
. 
├── .firebaserc             # Firebase project configuration
├── firebase.json           # Firebase project settings (hosting, functions, etc.)
├── firestore.indexes.json  # Firestore index definitions
├── firestore.rules         # Firestore security rules
├── storage.rules           # Firebase Storage security rules
├── database.rules.json     # Firebase Realtime Database rules
├── package.json            # Root project dependencies and scripts
├── package-lock.json       # Dependency lock file
├── functions/              # Firebase Cloud Functions
│   ├── index.js            # Main entry point for Cloud Functions
│   ├── package.json        # Functions dependencies
│   └── ...
├── public/                 # Static files for Firebase Hosting (frontend)
│   ├── admin-dashboard.html
│   ├── admin-login.html
│   ├── booking.html
│   ├── index.html
│   ├── images/             # Image assets
│   └── ...                 # Other HTML, CSS, and JS files
├── dataconnect/            # Data Connect related files (if used)
├── dataconnect-generated/  # Generated files for Data Connect
└── ...
```

## Author

**Thanniru Sai Teja**
*   Email: iamsaitejathanniru@gmail.com
*   LinkedIn: [https://www.linkedin.com/in/thannirusaiteja](https://www.linkedin.com/in/thannirusaiteja)

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details.
