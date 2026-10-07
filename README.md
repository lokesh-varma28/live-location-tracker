# 📍 Live Location Tracker

A real-time live location tracking web application built with **Node.js, Express.js, Socket.IO, and Leaflet.js**.

The application uses the browser's **Geolocation API** to capture the user's current location and updates it in real time on an interactive map using **Socket.IO**.

## ✨ Features

* 📍 Real-time GPS location tracking
* 🗺️ Interactive map using Leaflet.js
* ⚡ Real-time updates using Socket.IO
* 🌐 Browser-based Geolocation API
* 👤 Unique user/target identification
* 🔄 Automatic location updates
* 📱 Responsive web interface
* 🔐 Basic login-protected map access
* 🌍 Optional Cloudflare Tunnel support for public access

## 🛠️ Tech Stack

### Frontend

* HTML5
* CSS3
* JavaScript
* Leaflet.js
* OpenStreetMap

### Backend

* Node.js
* Express.js
* Socket.IO

### APIs & Tools

* Browser Geolocation API
* Cloudflared
* Nodemon

## 📂 Project Structure

```text
live-location-tracker/
│
├── public/
│   ├── map.html
│   ├── weather.html
│   ├── styles.css
│   └── script.js
│
├── views/
│   └── home.html
│
├── config.js
├── router.js
├── server.js
├── package.json
├── package-lock.json
└── README.md
```

## 🚀 Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/YOUR-USERNAME/live-location-tracker.git
```

### 2. Open the project

```bash
cd live-location-tracker
```

### 3. Install dependencies

```bash
npm install
```

### 4. Start the development server

```bash
npm run dev
```

The application will start on the configured local port.

For example:

```text
http://localhost:6589
```

## 🔐 Login Credentials

The current project uses the following default login credentials:

```text
Username: admin
Password: admin
```

After starting the application, open the local URL in your browser and use these credentials to access the protected pages.

> ⚠️ These are demo credentials for development/testing purposes. Change them before using the application in a production environment.

## ▶️ Production Start

To run the application without Nodemon:

```bash
npm start
```

## 📍 How It Works

1. Start the application using `npm run dev`.
2. Open the application in your browser.
3. Login using the demo credentials.
4. Open the location tracking page.
5. Allow the browser to access your location.
6. The browser obtains your latitude and longitude using the Geolocation API.
7. The location is sent to the Node.js server.
8. Socket.IO broadcasts the updated location in real time.
9. The location appears on the interactive Leaflet map.

```text
Browser
   │
   │ GPS Coordinates
   ▼
Express Server
   │
   │ Real-time events
   ▼
Socket.IO
   │
   ▼
Leaflet Map
   │
   ▼
Live Location
```

## 🗺️ Map

This project uses:

* **Leaflet.js** for the interactive map
* **OpenStreetMap** for map tiles

No Google Maps API key is required for the default map configuration.

## 💾 Data Storage

This version does **not use a permanent database**.

Active location data is temporarily maintained by the Node.js server while it is running.

> Restarting the server clears the temporary location data.

## 🌐 Public Access with Cloudflare Tunnel

The project can optionally use **Cloudflared** to expose the local server through a temporary public URL.

This is useful when testing location sharing between different devices or networks.

## ⚠️ Location Privacy

This application uses the browser's Geolocation API.

Users must explicitly grant location permission before their location can be accessed.

Do not use or share location data without the user's knowledge and consent.

## 🔧 Available Commands

### Install dependencies

```bash
npm install
```

### Development

```bash
npm run dev
```

### Production

```bash
npm start
```

## 👨‍💻 Author

**Lokesh Varma**

Full-Stack Developer

* GitHub: https://github.com/lokesh-varma28
* LinkedIn: https://www.linkedin.com/in/natra-lokesh-493bb63a2/
* Portfolio: https://my-portfolio-one-gold-42.vercel.app/

## 📄 License

This project is available for educational and personal development purposes.
