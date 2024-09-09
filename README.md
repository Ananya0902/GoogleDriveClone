
# Google Drive Clone

A fully functional Google Drive Clone built using **React.js** for the frontend and **Firebase** for authentication and storage management. This project replicates key features of Google Drive, allowing users to upload, store, organize, and manage files securely in a cloud environment.

## Features

- **User Authentication**: Secure authentication with Google using Firebase Authentication.
- **File Upload**: Upload multiple files simultaneously to Firebase Storage.
- **Folder Management**: Create, organize, and navigate through folders.
- **Real-time Updates**: Automatically updates file and folder changes in real-time.
- **File Sharing**: Share files with unique URLs.
- **Responsive Design**: Optimized for mobile and desktop views.
- **File Preview**: Preview images and documents directly within the app.
- **Storage Management**: View file details including size, type, and date uploaded.

## Tech Stack

### Frontend:
- **React.js**: Component-based UI library for building the interface.
- **React Router**: Handles routing between different views (e.g., home, folders).
- **Firebase Auth**: For handling user authentication.
- **CSS3**: Styling the user interface with responsive layouts.

### Backend:
- **Firebase**: Used for authentication, real-time database, and cloud storage.
  - **Firebase Authentication**: To authenticate users through Google Sign-In.
  - **Firebase Firestore**: To store metadata for uploaded files and folder structures.
  - **Firebase Storage**: To store user files in a scalable cloud environment.

## Project Setup

### Prerequisites

Before you can run this project, make sure you have the following installed:

- [Node.js](https://nodejs.org/)
- [Firebase Account](https://firebase.google.com/) with a new project set up

### Installation

1. **Clone the Repository:**
   ```bash
   git clone https://github.com/Ananya0902/GoogleDriveClone.git
   cd GoogleDriveClone
   ```

2. **Install Dependencies:**
   ```bash
   npm install
   ```

3. **Firebase Configuration:**

   - Go to your Firebase console and create a new project.
   - Enable **Authentication** (Google Sign-In method) and **Firebase Storage**.
   - Enable **Firestore** for managing file metadata.
   - In the root of the project, create a `.env` file to store Firebase configuration:
     ```bash
     REACT_APP_FIREBASE_API_KEY=<YOUR_FIREBASE_API_KEY>
     REACT_APP_FIREBASE_AUTH_DOMAIN=<YOUR_FIREBASE_AUTH_DOMAIN>
     REACT_APP_FIREBASE_PROJECT_ID=<YOUR_FIREBASE_PROJECT_ID>
     REACT_APP_FIREBASE_STORAGE_BUCKET=<YOUR_FIREBASE_STORAGE_BUCKET>
     REACT_APP_FIREBASE_MESSAGING_SENDER_ID=<YOUR_FIREBASE_MESSAGING_SENDER_ID>
     REACT_APP_FIREBASE_APP_ID=<YOUR_FIREBASE_APP_ID>
     ```

4. **Start the App:**
   ```bash
   npm start
   ```
   The app should now be running on `http://localhost:3000/`.

## Folder Structure

```bash
.
├── public
│   ├── index.html        # Main HTML file
├── src
│   ├── components        # Reusable React components (FileList, Navbar, etc.)
│   ├── context           # Firebase context provider
│   ├── hooks             # Custom React hooks (useAuth, useFirestore, etc.)
│   ├── pages             # Different pages (Dashboard, Login, etc.)
│   ├── App.js            # Main application file
│   ├── index.js          # React DOM rendering
├── .env                  # Environment variables (Firebase keys)
├── .gitignore            # Files to be ignored by Git
├── README.md             # Project documentation
├── package.json          # Project dependencies and scripts
└── firebase.js           # Firebase configuration and initialization
```

## Key Components

### 1. **Authentication (`useAuth.js`):**
   - Handles user authentication logic, including Google Sign-In using Firebase.

### 2. **File Upload (`UploadFile.js`):**
   - Enables users to upload files to Firebase Storage and store metadata in Firestore.

### 3. **File Listing (`FileList.js`):**
   - Dynamically displays a list of uploaded files and folders in a tree-like structure.

### 4. **Folder Navigation (`Folder.js`):**
   - Allows users to navigate between different folders and manage their files.


## Future Enhancements

- **Search Functionality**: Implement a search bar to quickly find files and folders.
- **File Sorting**: Add sorting options (e.g., by name, date, size).
- **File Sharing**: Provide options for file permission control and sharing.
- **Pagination**: Efficiently handle large numbers of files with pagination.

## Contributing

If you'd like to contribute to this project, feel free to submit a pull request or file an issue. Contributions are always welcome!


## Contact

If you have any questions or suggestions, feel free to reach out!

- **Author**: Ananya Srivastava
- **Email**: ananyasrivastava@example.com
- **GitHub**: [Ananya0902](https://github.com/Ananya0902)
