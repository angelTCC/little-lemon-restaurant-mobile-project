# 🍋 Little Lemon App

A mobile app for a Mediterranean restaurant with a **React Native + Expo frontend** and a **Node.js + MySQL backend** running locally in Docker containers. The app supports offline menu browsing via SQLite.

## 🚀 Project Overview

Little Lemon lets users browse and filter the restaurant menu, manage profiles, and enjoy a seamless experience.

## 📂 Repositories

* **Frontend:** [little-lemon-frontend](https://github.com/yourusername/little-lemon-frontend)
  React Native app using Expo, SQLite for local caching, and UI features.

* **Backend:** [little-lemon-backend](https://github.com/yourusername/little-lemon-backend)
  Node.js REST API with MySQL database, Dockerized for local development and testing.


## 📱 Frontend Features

* Onboarding screen (name + email)
* Full menu browsing and category filtering
* Search with loading indicators
* Profile management
* Offline menu access with SQLite
* Published on Google Play Store (frontend only)
* Connects to backend API (hosted locally for now)

## 🖥️ Backend Features

* REST API server for menu and user data
* MySQL database running inside Docker
* Runs locally with exposed ports for app connectivity
* Authentication planned for later implementation


## 🐳 Docker Setup (Backend)

* Uses Docker Compose to manage Node.js and MySQL containers
* Easy setup and teardown on any machine with Docker installed
* Ports exposed for frontend-backend communication

## ⚙️ Development Setup

### Backend

1. Clone: `git clone https://github.com/yourusername/little-lemon-backend.git`
2. Run: `docker-compose up`
3. Use port forwarding or ngrok for external access if needed.

### Frontend

1. Clone: `git clone https://github.com/yourusername/little-lemon-frontend.git`
2. Install: `npm install`
3. Start: `expo start`
4. Configure API base URL to point to backend server IP or tunnel URL.

## 📅 Roadmap

| Phase            | Description                                     |
| ---------------- | ----------------------------------------------- |
| MVP              | Frontend with onboarding, menu, search, offline |
| Backend Setup    | Local Dockerized API + MySQL database           |
| Authentication   | Add Firebase/custom auth                        |
| Publishing       | Publish frontend app to Google Play             |
| Cloud Deployment | Deploy backend to cloud service                 |


## 📞 Contact

For questions or contributions, contact Angel Chaico.

