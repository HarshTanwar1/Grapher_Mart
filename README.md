<div align="center">

# 📸 Grapher Mart

A two-sided marketplace that connects photographers with the customers who want to hire them

Photographers build a profile, tag the shoots they offer, and showcase a portfolio.
Customers browse, filter by category & location, view work, and **chat in real time** to book a shoot

<br/>

![React](https://img.shields.io/badge/React-17-61DAFB?style=for-the-badge&logo=react&logoColor=black)
![Firebase](https://img.shields.io/badge/Firebase-8-FFCA28?style=for-the-badge&logo=firebase&logoColor=black)
![Material UI](https://img.shields.io/badge/Material--UI-4-007FFF?style=for-the-badge&logo=mui&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-ES6+-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![React Router](https://img.shields.io/badge/React_Router-5-CA4245?style=for-the-badge&logo=reactrouter&logoColor=white)

</div>

<br/>

## ✨ Highlights

- ⚡ **Real-time chat** between customers and photographers, powered by Cloud Firestore live listeners.
- 🔐 **Full auth flow** for two distinct user roles (photographers & customers) using Firebase Authentication.
- 🖼️ **Multi-image uploads** to Cloud Storage with live portfolio management (add / remove / set profile photo).
- 🔎 **Smart discovery** — filter photographers by 20+ categories, state, and city, or search by name.
- 🚫 **Serverless architecture** — the entire backend (auth, database, storage) runs on Firebase, no custom server required.

<br/>

## 🛠️ Tech Stack

| Layer              | Technologies                                              |
| ------------------ | --------------------------------------------------------- |
| **Frontend**       | React 17, React Router DOM v5                             |
| **UI**             | Material-UI v4, Bootstrap / React-Bootstrap, react-select |
| **Backend (BaaS)** | Firebase Authentication, Cloud Firestore, Cloud Storage   |
| **Utilities**      | country-state-city, react-flip-move, react-loader-spinner |
| **Tooling**        | Create React App                                          |

<br/>

## 🚀 Features

### 👤 For Photographers

- **Sign up / log in** with email and password.
- **Guided onboarding** — pick from 20+ categories (Wedding, Birthday, Fashion, Drone, Maternity, and more), upload a profile picture, and add sample work.
- **Personal dashboard** showing your public profile: name, contact details, location, categories, and portfolio.
- **Edit anything** — update details, manage categories, add/remove portfolio photos, and change your profile picture.
- **Messages inbox** — view every customer conversation and reply in real time.

### 🧑‍💻 For Customers

- **Sign up / log in** with email and password.
- **Browse photographers** in a card-based feed with a preview of each one's sample work.
- **Filter** by category, state, and city, or **search** by name.
- **View full profiles** with the complete portfolio and selected categories.
- **Chat in real time** to discuss and arrange a shoot.

<br/>

## ⚙️ Getting Started

```bash
# 1. Clone the repository
git clone https://github.com/HarshTanwar1/Grapher_Mart.git
cd Grapher_Mart

# 2. Install dependencies
npm install

# 3. Start the development server
npm start
```

The app runs at **[http://localhost:3000](http://localhost:3000)** and reloads automatically on edits.

> **Configuring your own Firebase:** update the config in [src/firebase.js](src/firebase.js) with your project credentials, then enable **Email/Password Authentication**, **Cloud Firestore**, and **Cloud Storage** in the Firebase console

<br/>

## 🧠 What I Learned

- **Firebase as a complete backend** — wiring Authentication, Firestore, and Cloud Storage together, and using `onAuthStateChanged` to gate protected pages.
- **Real-time data** — building live chat with Firestore `onSnapshot` listeners and `serverTimestamp()`, and deriving a deterministic conversation ID from both participants' UIDs.
- **File handling** — uploading multiple images to Cloud Storage, tracking upload tasks, fetching download URLs, and keeping Firestore in sync with `arrayUnion` / `arrayRemove`.
- **Client-side routing** — structuring a multi-page SPA with React Router, including passing state between routes.
- **Complex form state** — managing multi-step forms, conditional view/edit modes, and dependent dropdowns (picking a state populates its cities) with React hooks.
- **Composing third-party UI libraries** — building responsive layouts with Material-UI's Grid, Paper, AppBar, and form components.

<br/>

## 🔮 Future Improvements

- 📅 **Booking & scheduling** so customers can request and confirm shoots, not just chat.
- ⭐ **Reviews and ratings** to build trust between users.
- 📱 **Responsive redesign** — replace fixed `vw`/`vh` units with a fluid, mobile-friendly layout.
- 🧱 **Modern SDKs** — migrate to the modular Firebase v9+ SDK and upgrade to MUI v5+ for smaller bundles.
- ✅ **Robustness** — add input validation, error boundaries and loading/error states.
- 🌍 **Global location support** — generalize the currently India-only state/city filtering.

<br/>

---

<div align="center">

⭐ _If you found this project helpful or interesting, consider giving it a star!_ ⭐

</div>
