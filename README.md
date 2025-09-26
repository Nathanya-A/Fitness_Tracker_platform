## 🏋️‍♀️ FITTRACK - Fitness Tracker 

A full-stack web application that helps users **plan, track, and analyze their daily workouts**.  
Built with the **MERN stack**—MongoDB, Express.js, React, and Node.js.

### ✨ Features
- **User Authentication**: Secure sign-up/login with JWT and bcrypt password hashing.
- **Workout Management**: Add exercises, sets, reps, and calories burned.
- **Progress Dashboard**: Visualize weekly/monthly performance with interactive charts.
- **Responsive Design**: Works smoothly on desktop, tablet, and mobile devices.

---

### 🛠️ Tech Stack
**Frontend**
- React, React Router, Redux (or Context)
- Styled-Components / Tailwind CSS
- Chart.js for analytics

**Backend**
- Node.js
- Express.js REST API
- MongoDB Atlas (Mongoose ODM)

**Other Tools**
- Netlify (frontend) & Render (backend) for deployment
- Git for version control

---

### 🏗️ Architecture
```text
React Client  <---->  Express REST API  <---->  MongoDB Database
```

- **Client** sends JSON requests (Axios/Fetch)  
- **Server** validates & processes requests, returns JSON responses  
- **Database** stores user profiles, workouts, and exercise details  

---

### 📷 User Interface

![Signup.png](https://github.com/Nathanya-A/Fitness_Tracker_platform/blob/master/Signup.PNG)
![Dashboard.png](https://github.com/Nathanya-A/Fitness_Tracker_platform/blob/master/Dashboard.PNG)
![Workoutpng](https://github.com/Nathanya-A/Fitness_Tracker_platform/blob/master/Workout.PNG)

---

### 🚀 Getting Started

#### Prerequisites
- Node.js (v18+ recommended)
- npm or yarn
- MongoDB Atlas account (or local MongoDB)
- React.js

#### Clone the Repo
```bash
git clone https://github.com/your-username/Fitness_Tracker_platform.git
cd Fitness_Tracker_platform
```
#### Setup Environment for MERN Stack
- Install Node.js
- Install MongoDB
- **Install dependencies**
  - Backend
    ```bash
    cd server
    npm init
    npm install bcrypt cors dotenv express jsonwebtoken mongoose nodemon
    ```
  - Frontend
    ```bash
    cd client
    npm start
    npm install styled-components @mui/material @mui/lab @mui/icons-material @emotion/styled @emotion/react axios react-router-dom react-redux redux-persist @reduxjs/toolkit dayjs @mui/x-charts @mui/x-date-pickers
  ```
---

### 🗄️ Database Management

The project uses **MongoDB Atlas** (cloud-hosted) for scalability and easy deployment.  
You can also run a **local MongoDB instance** if preferred.

##### Create a Cluster (MongoDB Atlas)
1. Sign up at [MongoDB Atlas](https://www.mongodb.com/atlas).
2. Click **Build a Cluster** → choose the **Free Tier (M0)** or a paid tier if needed.
3. Select a cloud provider & region closest to your users.
4. Wait a few minutes while Atlas provisions the cluster.

##### Create a Database User
1. Go to **Database Access** → **Add New Database User**.
2. Choose **Password Authentication**.
3. Assign a strong username and password.
4. Give the user **Read and Write to Any Database** (or more restrictive roles as needed).

##### Configure Network Access
1. In **Network Access**, click **Add IP Address**.
2. To allow local development, use `0.0.0.0/0` (all IPs) or specify your public IP for tighter security.

##### Get Your Connection String
1. In **Clusters**, click **Connect** → **Connect Your Application**.
2. Copy the **MongoDB URI**, which will look like:
```bash
mongodb+srv://<username_db>:<password_db>@cluster1.acxeilv.mongodb.net/?retryWrites=true&w=majority&appName=Cluster1
```
3. Replace `<username_db>` and `<password_db>` with the database user credentials you created.

---

### 🔑 Environment Variables
Create a `.env` file in the server directory with
```bash
PORT = 8080
MONGO_URI = your_mongodb_connection_string
JWT_SECRET = your_jwt_secret
```

**Run Development Server**
```bash
# Backend
cd server
npm run dev

# Frontend
cd client
npm start
```
The app will be locally available at:
- Backend: http://localhost:8080
- Frontend: http://localhost:3000

---

### 🌐 Deployment
- **Frontend:** [Netlify](https://www.netlify.com/)
- **Backend:** [Render](https://render.com/) or [Heroku](https://www.heroku.com/)
- Set environment variables in your hosting dashboard.

--- 

### 🔮 Future Enhancements
- Built-in workout **tutorials** with step-by-step guidance
- Blog section for fitness tips, nutrition advice, and community posts
- Social features for sharing progress with friends
- Integration with wearable devices (Fitbit, Apple Health)
- AI-based workout recommendations
- Progressive Web App (PWA) for offline support
    
 
    
