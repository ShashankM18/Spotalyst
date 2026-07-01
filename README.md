# 🌍 Spotalyst

A comprehensive web application for discovering, managing, and planning visits to amazing places around the world. Built with React, Node.js, Express, and MongoDB.

## ✨ Features

### 🔍 Smart Location Search
- **Intelligent Autocomplete**: Real-time location suggestions using LocationIQ API
- **Place & City Search**: Separate search for places and cities with auto-suggestions
- **Global Coverage**: Search for locations worldwide

### ⏰ Advanced Time Planning
- **Duration Planning**: Set recommended visit duration in hours
- **Start Time Scheduling**: Plan your visit start time
- **Operating Hours**: Track opening and closing times
- **Smart Conflict Detection**: Automatic warnings for timing conflicts
- **Visual Time Validation**: Color-coded feedback for timing feasibility

### 🎯 Audience Targeting
- **Multiple Audience Types**: Family, Friends, Couples, Solo Travelers, etc.
- **Personalized Recommendations**: Tailored suggestions based on audience
- **Flexible Categories**: Heritage, Religious, Adventure, Nature, Cultural, Food, Shopping, Entertainment

### 📱 Modern User Interface
- **Responsive Design**: Works seamlessly on desktop, tablet, and mobile
- **Beautiful Gradients**: Eye-catching color schemes and animations
- **Interactive Elements**: Hover effects, smooth transitions, and micro-interactions
- **Bootstrap Integration**: Professional styling with custom enhancements

### 📊 Data Management
- **CRUD Operations**: Create, Read, Update, Delete spots
- **Real-time Updates**: Instant reflection of changes
- **Data Persistence**: MongoDB integration for reliable storage
- **Email Tracking**: Associate spots with user email addresses

## 🛠️ Tech Stack

### 🖥️ Frontend
- **React 18.2.0** – Component-based UI library for building dynamic interfaces
- **Bootstrap 5.3.1** – Responsive CSS framework for layout and styling
- **Axios 1.5.0** – Promise-based HTTP client for RESTful API communication
- **LocationIQ API** – Geolocation API for location autocomplete and place data

### 🛠️ Backend
- **Node.js** – JavaScript runtime for server-side development
- **Express 4.18.2** – Lightweight web framework for building REST APIs
- **MongoDB** – NoSQL document database to store tourist spot data
- **Mongoose 7.5.0** – ODM for MongoDB to manage schemas and models
- **CORS 2.8.5** – Middleware to handle cross-origin requests
- **dotenv 16.3.1** – Environment variable configuration

### 🤖 AI & Automation (n8n Workflow)
- **n8n (Self-hosted)** – Low-code automation platform integrated with backend:
    - **Webhook Trigger** – Receives input from website form submission
    - **OpenAI GPT API** – Generates personalized, context-aware travel itineraries
    - **Email Node** – Automatically sends the generated itinerary to the user’s email
    - Fully automated from form submission to itinerary generation and delivery

### ⚙️ Development Tools
Nodemon 3.0.1 – Auto-restarts backend server on file changes
Concurrently 8.2.0 – Runs frontend and backend servers in parallel
React Scripts 5.0.1 – Build and development tools for React

## 📋 Prerequisites

Before running this application, make sure you have:

- **Node.js** (v14.0.0 or higher)
- **npm** (v6.0.0 or higher)
- **MongoDB** account and cluster
- **LocationIQ** API key (free tier available)



The application will be available at:
- **Frontend**: http://localhost:3000
- **Backend API**: http://localhost:5000

## 📁 Project Structure

```
spot-explorer/
├── client/                 # React frontend
│   ├── public/
│   │   └── index.html
│   ├── src/
│   │   ├── App.js         # Main React component
│   │   ├── App.css        # Component styles
│   │   ├── index.js       # React entry point
│   │   └── index.css      # Global styles
│   └── package.json       # Client dependencies
├── controllers/           # Express route controllers
│   └── spotController.js  # Spot CRUD operations
├── models/               # MongoDB schemas
│   └── Spot.js          # Spot data model
├── routes/              # Express routes
│   └── spotRoutes.js    # Spot API routes
├── .env                 # Environment variables
├── .gitignore          # Git ignore rules
├── package.json        # Server dependencies
├── server.js           # Express server setup
└── README.md           # Project documentation
```

## 🔌 API Endpoints

### Spots
- `GET /api/spots` - Get all spots
- `POST /api/spots` - Create a new spot
- `PUT /api/spots/:id` - Update a spot
- `DELETE /api/spots/:id` - Delete a spot
- `POST /api/spots/bulk` - Bulk insert spots


---

⭐ **Star this repository if you found it helpful!**
