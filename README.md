# Smart Section Management (SSM) — Frontend Client

[![Live Demo](https://img.shields.io/badge/Live%20Demo-diussm.vercel.app-00dfa2?style=flat-square&logo=vercel)](https://diussm.vercel.app)
[![React](https://img.shields.io/badge/React-19-61dafb?style=flat-square&logo=react)](https://react.dev/)
[![Vite](https://img.shields.io/badge/Vite-Build%20Tool-646cff?style=flat-square&logo=vite)](https://vitejs.dev/)
[![Tailwind CSS](https://img.shields.io/badge/Tailwind-CSS%20v4-38bdf8?style=flat-square&logo=tailwindcss)](https://tailwindcss.com/)
[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg?style=flat-square)](LICENSE)

> A modern, responsive web application engineered for university academic coordination. Streamlines course section scheduling, student rosters, task assignments, and department communication.

**Live Application:** [https://diussm.vercel.app](https://diussm.vercel.app)  
**Backend Repository:** [banrayndox/ssm-backend](https://github.com/banrayndox/ssm-backend)

---

## 📌 Overview

**Smart Section Management (SSM)** is a comprehensive web platform built specifically to resolve the logistical friction of course section allocations, class coordination, and academic announcements in university environments.

It replaces disorganized social media group chats with an organized, role-based dashboard where **Authorities**, **Teachers**, **Class Representatives (CRs)**, and **Students** collaborate in real-time.

---

## 🚀 Key Features

### 🏛️ Authority / Admin Portal
* **Department & Batch Management:** Configure academic departments, semesters, and intake batches.
* **Course & Section Catalog:** Add, update, and manage official course offerings and sectional rosters.
* **Teacher & CR Assignment:** Assign course teachers and officially designate Class Representatives.

### 🎓 Teacher Portal
* **Course Control:** Manage teaching rosters and view enrolled students.
* **Lecture Scheduling:** Announce class schedules, exam dates, and passkey-protected enrollments.
* **Direct Notices:** Push announcements directly to specific course sections.

### 📢 Class Representative (CR) Tools
* **Roster Management:** View assigned and unassigned student lists for timely coordination.
* **Task Management:** Distribute and track section assignments, deadlines, and project submissions.
* **Polls & Notices:** Create interactive polls to vote on make-up class slots and post urgent class updates.

### 👤 Student / User Portal
* **Section Enrollment:** Submit requests to join course sections with real-time status tracking.
* **Central Notice Board:** Access verified notices, exam timetables, and interactive polls.
* **Issue Reporting:** Submit administrative issues and course grievances directly to section coordinators.

---

## 🛠️ Technology Stack

* **Framework:** [React 19](https://react.dev/)
* **Build Tool:** [Vite](https://vitejs.dev/)
* **Styling:** [Tailwind CSS v4](https://tailwindcss.com/)
* **Routing:** [React Router v7](https://reactrouter.com/)
* **HTTP Client:** [Axios](https://axios-http.com/)
* **Icons & Notifications:** [React Icons](https://react-icons.github.io/react-icons/), [React Hot Toast](https://react-hot-toast.com/)
* **Deployment:** [Vercel](https://vercel.com/)

---

## 📁 Project Architecture

```
ssm-frontend/
├── public/               # Static assets & branding
├── src/
│   ├── assets/           # Local datasets & media
│   ├── components/       # Reusable UI & role-based components
│   │   ├── Authority/    # Admin course/section/user management
│   │   ├── CR/           # CR task distribution, student lists & polls
│   │   ├── Teacher/      # Teacher course & exam management
│   │   └── User/         # Student notice, poll & request forms
│   ├── helper/           # Axios API service configuration
│   ├── pages/            # Page-level route views (Authority, CR, User, Auth)
│   ├── store/            # Global context & state management (AppContext)
│   ├── App.jsx           # Main routing declaration
│   ├── index.css         # Tailwind CSS entry
│   └── main.jsx          # React DOM root entry
├── package.json
└── vite.config.js
```

---

## ⚙️ Getting Started

### Prerequisites
* **Node.js:** v18.0.0 or higher
* **npm:** v9.0.0 or higher

### Installation

1. **Clone the repository:**
   ```bash
   git clone https://github.com/banrayndox/ssm-frontend.git
   cd ssm-frontend
   ```

2. **Install dependencies:**
   ```bash
   npm install
   ```

3. **Configure Environment Variables:**
   Create a `.env` file in the root directory:
   ```env
   VITE_API_BASE_URL=http://localhost:5000/api
   ```
   *(For production, point this to your deployed backend API URL).*

4. **Run Development Server:**
   ```bash
   npm run dev
   ```
   The client will be running at `http://localhost:5173`.

5. **Build for Production:**
   ```bash
   npm run build
   ```

---

## 🔗 Related Repositories

* **Backend API:** [banrayndox/ssm-backend](https://github.com/banrayndox/ssm-backend)

---

## 👨‍💻 Author

**Rakib B**
* GitHub: [@banrayndox](https://github.com/banrayndox)
* Website: [banrayndox.github.io](https://banrayndox.github.io/)
* Institution: Daffodil International University (DIU)

---

## 📄 License

This project is licensed under the [MIT License](LICENSE).
