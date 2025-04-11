
# 🎵 Innovators Hub Music

**Innovators Hub Music** is a feature-rich music streaming web application built using **ReactJS** and backed by **Firebase**. It allows users to register, log in, manage their profiles, and stream music seamlessly. It also includes an admin dashboard for uploading and managing albums and tracks.

---

## 🚀 Features

### 🔐 Authentication
- **Login**, **Register**, and **Forgot Password** with Firebase Auth
- Secure and real-time user session management

### 👤 User Profile
- Update **profile picture** and **personal details**
- Option to **delete account**
- Data managed through **Firebase Firestore & Storage**

### 🎧 Music Experience
- **Home Page** shows all uploaded albums
- **Album Details** and **Song List** view
- In-app music playback
- Smooth, responsive UI with reusable components

### 🧑‍💼 Admin Dashboard
- Protected route for admin access
- Upload new albums and manage song listings

---

## 🛠️ Tech Stack

- **Frontend:** ReactJS, React Router, TailwindCSS (or CSS)
- **Backend:** Firebase (Authentication, Firestore, Storage)
- **State Management:** React Context API
- **Other Tools:** Vite, Toastify (optional for alerts), PostCSS

---

## 📁 Folder Structure (Simplified)

```
src/
├── admin/            # Admin page (e.g., AddAlbum)
├── auth/             # Login, Register, Forgot Password
├── backend/          # Firebase config
├── components/       
│   ├── home/         # Dashboard, AlbumDetails, SongList
│   └── helpers/      # Utility components like Spinner
├── context/          # Auth & Album context providers
├── user/             # Profile & DeleteAccount
├── routes/           # React Router config
├── App.jsx
├── index.js
```

---

## 🔧 Getting Started

### 1. Clone the Repository

```bash
[git clone https://github.com/David4988/Innovators-Hub.git)](https://github.com/David4988/Innovators-Hub.git)
cd innovators-hub-music
```

### 2. Install Dependencies

```bash
npm install
```

### 3. Configure Firebase

- Create a project on [Firebase Console](https://console.firebase.google.com/)
- Enable:
  - **Email/Password Authentication**
  - **Firestore Database**
  - **Firebase Storage**
- Replace the Firebase config in `src/backend/firebaseConfig.js`

### 4. Run the App

```bash
npm run dev
```

---

## 🔐 Admin Role Setup

1. In Firebase **Firestore**, locate the user’s document.
2. Add the following field:

```json
"role": "admin"
```

3. The user will now have access to the admin page to add albums.

---

## 📬 Contact

**Developed by [Jason David](https://github.com/David4988)**  
📧 Email: davidson4988@gmail.com
🔗 LinkedIn: [Jason David](https://www.linkedin.com/in/david4988/)
