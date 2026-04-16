# Visitor Management System

A modern, free web application for managing and tracking office visitors.

## Features ✨
- **Dashboard**: Real-time statistics of visitors in the building
- **Check-In System**: Register visitors with automatic badge generation
- **Check-Out**: Easy visitor departure tracking
- **Visitor Records**: Search and filter visitor history
- **Host Management**: Add and manage office employees
- **Responsive Design**: Works on desktop and mobile devices

## Tech Stack 🛠️
- **Frontend**: React 18
- **Backend**: Node.js with Express
- **Database**: SQLite (no setup needed)
- **Styling**: CSS3 with responsive design

## Installation 📦
### Prerequisites
- Node.js (v14 or higher)
- npm or yarn

### Quick Start
1. Clone the repository:
   ```bash
   git clone https://github.com/alockt-maker/visitor-management-app.git
   cd visitor-management-app
   ```
2. Install dependencies:
   ```bash
   npm run install
   ```
3. Start the application:
   ```bash
   npm start
   ```
   The app will open at http://localhost:3000
   The backend runs on http://localhost:5000

## Project Structure 📁
visitor-management-app/
├── backend/
│   ├── server.js
│   ├── visitors.db
│   └── package.json
├── frontend/
│   ├── public/
│   │   └── index.html
│   ├── src/
│   │   ├── components/
│   │   │   ├── Dashboard.js
│   │   │   ├── CheckIn.js
│   │   │   ├── CheckOut.js
│   │   │   ├── VisitorList.js
│   │   │   └── HostManagement.js
│   │   ├── App.js
│   │   ├── App.css
│   │   └── index.js
│   └── package.json
└── README.md

## Usage 🚀
1. **Add Hosts/Employees**: Go to the Hosts tab and add office employees
2. **Check-In Visitors**: Use the Check-In tab to register new visitors
3. **View Visitor Records**: Go to Visitor List to see all visitor history
4. **Check-Out**: Use the Check-Out tab to mark visitors as departed
5. **Dashboard**: Monitor real-time statistics

## Database Schema 📊
### Hosts Table
- id (PRIMARY KEY)
- name
- email
- department
- created_at

### Visitors Table
- id (PRIMARY KEY)
- name
- email
- phone
- company
- purpose
- host_id (FOREIGN KEY)
- check_in_time
- check_out_time
- badge_number

## Deployment 🌐
### Free Hosting Options
- **Backend**: Render.com, Heroku
- **Frontend**: Vercel, Netlify, GitHub Pages

### Steps for Deployment
1. Push the code to GitHub
2. Connect your GitHub repo to Render (backend) and Vercel (frontend)
3. Set environment variables if needed
4. Deploy!

## API Endpoints 📡
GET /api/hosts - Get all hosts
POST /api/hosts - Add a new host
DELETE /api/hosts/:id - Delete a host
GET /api/visitors - Get all visitors
POST /api/visitors/check-in - Check in a visitor
POST /api/visitors/check-out/:id - Check out a visitor
GET /api/dashboard - Get dashboard statistics

## License 📄
MIT License

## Author 👨‍💻
alockt-maker
---
Made with ❤️ for better visitor management
