# 🍋 Little Lemon Mobile App

A mobile app for a Mediterranean restaurant built with React Native + Expo for the frontend, with a backend server (Node.js + MySQL) running locally in Docker containers. The app uses SQLite locally for offline menu access.

---

## 🚀 Project Overview

Little Lemon is designed to offer users a seamless way to browse the restaurant menu, filter dishes by category, and personalize their experience with onboarding and profile management.

---

## 📱 Frontend

* Built with React Native + Expo
* Uses SQLite for offline data storage and caching menu data
* Features include:

  * Onboarding screen for new users
  * Menu browsing and filtering
  * Search functionality with loading indicators
  * Profile management
* Published on Google Play Store (frontend only)
* Connects to backend API hosted on your local machine

---

## 🖥️ Backend

* Node.js REST API server serving menu data and handling user data
* MySQL database running inside a Docker container
* Backend server runs locally on your computer inside Docker containers
* Backend API exposed via port forwarding or ngrok to enable app connectivity
* Authentication planned for production phase (Firebase or custom auth)

---

## 🐳 Docker Setup

* Docker Compose manages the backend containers (Node.js API + MySQL)
* Simplifies environment setup and deployment on any machine with Docker installed
* Ports are exposed to allow frontend app to communicate with backend server

---

## ⚙️ Development Setup

### Prerequisites

* Node.js and npm installed
* Docker and Docker Compose installed
* Expo CLI installed globally (`npm install -g expo-cli`)

### Running Backend Locally

1. Clone the backend repository
2. Run `docker-compose up` to start the backend server and MySQL container
3. Configure your router for port forwarding or run `ngrok` to expose the backend API publicly
4. Update the frontend API base URL to point to your public IP or ngrok URL

### Running Frontend Locally

1. Clone the frontend repository
2. Run `npm install` to install dependencies
3. Run `expo start` to launch the app in Expo Go or simulator
4. The app connects to the backend API at the configured URL

---

## 🗂️ Repository Structure

```
/frontend
  ├── App.js
  ├── /screens
  ├── /assets
  └── package.json

/backend
  ├── docker-compose.yml
  ├── Dockerfile
  ├── /src
  │    ├── api.js
  │    ├── routes.js
  │    └── ...
  ├── /migrations
  ├── /models
  └── package.json
```

---

## 📅 Roadmap & Next Steps

| Phase            | Features/Tasks                                                                    |
| ---------------- | --------------------------------------------------------------------------------- |
| MVP (Current)    | Onboarding, menu browsing, filtering, offline cache, search, local SQLite storage |
| Backend setup    | Node.js + MySQL in Docker, API endpoints, local deployment                        |
| Authentication   | Implement Firebase auth or custom login system                                    |
| Publishing       | Release frontend to Google Play Store                                             |
| Cloud deployment | Future plan to deploy backend to cloud service                                    |

---

## 📞 Support & Contributions

Feel free to open issues or pull requests for improvements. For questions, contact Angel Chaico.
