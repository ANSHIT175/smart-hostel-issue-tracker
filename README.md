# Smart Hostel Issue Tracker

## Problem Statement
Hostel complaints like electricity, water, cleanliness, and internet issues are difficult to track and often get delayed due to lack of a transparent system.

## Solution
Smart Hostel Issue Tracker is a full-stack web application that allows students to raise hostel issues digitally and track their status in real time, while admins can manage, assign, and resolve complaints efficiently.

---

## Key Features

### Student Side
- Raise hostel issues easily using a simple form
- View issue status in real time  
  *(Reported → In Progress → Resolved)*
- Track previously raised complaints

### Admin Side
- View all student complaints
- Update issue status
- Manage reported vs resolved issues

---

## Tech Stack

- **Frontend:** React + Tailwind CSS  
- **Backend:** Node.js + Express  
- **Database:** MongoDB *(planned for production)*  

---

## Backend Architecture

The backend exposes REST APIs to manage hostel issues.

### API Flow
- **POST /api/issues** → Create a new issue  
- **GET /api/issues** → Fetch all issues  
- **PATCH /api/issues/:id** → Update issue status  

### Data Handling
Currently, issues are stored **in-memory** for demo purposes.  
This allows fast iteration and a clear API demonstration.

In production, this layer will be replaced with **MongoDB** for persistent storage and scalability.

---

## Live Demo

### Frontend (Deployed)
https://frontend-pi-snowy-63.vercel.app/

### Backend API
https://issue-tracker-backend-anshitpandey958.replit.app

---

## Demo Video
The working demo video showcases:
- Student raising an issue
- Issue appearing in the dashboard
- Status change flow
- Backend API calls visible via browser DevTools

*(Submitted separately as part of the hackathon submission)*

---

## How to Run Locally

### Prerequisites
- Node.js (v18+)

### Steps
1. Clone the repository  
2. Install dependencies  
   ```bash
   npm install

cd server
npm run dev
cd client
npm run dev

