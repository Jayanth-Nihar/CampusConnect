# CampusConnect
Campus Connect is a student collaboration platform that helps freshmen seek mentorship, find events/workshops, discover hackathon teammates, swap skills, and connect via anonymous chats.  This project aims to simplify campus networking and collaboration.

## 🌟 Features

1. **Freshman–Senior Connect (Mentorship Hub)**  
   - Freshmen can connect with seniors and alumni for guidance.  
   - Mentorship recommendations based on skills and interests.  
   - Role-based onboarding: Freshman | Senior | Alumni.

2. **Events & Opportunities Hub**  
   - Centralized hub for **workshops, hackathons, and campus events**.  
   - Filters: category, skills, online/offline events.  
   - Bookmark and track events you’re interested in.

3. **Skill Swap & Team Finder**  
   - Post what skills you can **teach** and what skills you want to **learn**.  
   - Create hackathon/project posts to find teammates.  
   - Connect students with complementary skills for collaboration.

4. **Anonymous Chat**  
   - Ask questions and engage in discussions without revealing your identity.  
   - Global “Anonymous Lounge” and 1:1 anonymous chats.  
   - Safe messaging with moderation and reporting.

---

## 🛠️ Tech Stack

- **Frontend:** HTML, CSS, JavaScript  
- **Backend:** Node.js + Express.js  
- **Database:** MongoDB (Atlas or local)  
- **Version Control:** GitHub  

---

## 📂 Project Structure

CampusConnect/
│── frontend/ # HTML, CSS, JS files for UI
│── backend/ # Node.js + Express.js APIs
│── database/ # MongoDB models and schemas
│── README.md # Project documentation
│── package.json # Dependencies


## 👥 Team Members- MENTOR(KARTHIK SRIRAMOJU)

- Abhiram Modukuru 
-Jayanth NIhar
-Siddartha ammika
- Karthik.A

  

---

## 🚀 Getting Started

### 1. Clone the repo
```bash
git clone https://github.com/your-username/CampusConnect.git
cd CampusConnect
2. Install dependencies
bash
Copy code
npm install
3. Setup MongoDB
Create a MongoDB Atlas cluster or use local MongoDB.

Add your connection URI in a .env file:

env
Copy code
MONGO_URI=your_mongo_connection_string
PORT=5000
4. Run the server
bash
Copy code
node backend/server.js
5. Open the frontend
Open frontend/index.html in your browser to view the landing page.

⚡ Contribution Guidelines
Branching: Each feature should have its own branch:

bash
Copy code
git checkout -b feature-name
Commit: Write clear commit messages.

Pull Request: Open PR to main branch after finishing a feature.

Code Review: Team lead reviews before merging.

📌 Roadmap
 GitHub repo setup

 Build landing page (HTML/CSS)

 User Auth & Profiles (Freshman/Senior/Alumni)

 Events Hub with filters & bookmarks

 Skill Swap & Team Finder

 Anonymous Chat with reporting

 Testing & UI polish

 Hackathon demo preparation

📜 License
This project is licensed under the MIT License.

💡 Vision
To bridge the gap between freshmen, seniors, and alumni, make campus opportunities visible, encourage skill-sharing, and create a safe environment for students to ask questions and collaborate freely.

# 🎓 CampusConnect - Student Networking Platform

> **Freshman–Senior Connect Platform** | Built by students, for students

## 📋 Project Overview

CampusConnect is a comprehensive student networking platform that bridges the gap between freshmen, seniors, and alumni through mentorship, events, skill sharing, and anonymous discussions.

### 🎯 Core Features
- **👨‍🏫 Seniors' Guidance & Mentorship** - Connect freshmen with experienced seniors
- **📅 Events & Opportunities Board** - Discover workshops, hackathons, and campus events
- **🤝 Skill Swap + Teammates Finder** - Find project partners and learn new skills
- **🕵️ Anonymous Chat** - Safe, moderated discussions for sensitive topics

## 🚀 Quick Start

### Prerequisites
- Node.js (v16+)
- MongoDB (local or Atlas)
- Git

### Installation
```bash
# Clone the repository
git clone <your-repo-url>
cd campusconnect

# Install backend dependencies
cd backend
npm install

# Install frontend dependencies
cd ../frontend
npm install

# Set up environment variables
cp .env.example .env
# Edit .env with your MongoDB URI and JWT secret
```

### Running the Application
```bash
# Terminal 1: Start backend server
cd backend
npm run dev

# Terminal 2: Start frontend development server
cd frontend
npm start
```

Visit `http://localhost:3000` to see the application.

## 📁 Project Structure
```
campusconnect/
├── backend/                 # Node.js + Express API
│   ├── controllers/        # Route handlers
│   ├── models/            # MongoDB schemas
│   ├── routes/            # API endpoints
│   ├── middleware/        # Auth, validation
│   └── server.js          # Main server file
├── frontend/              # React application
│   ├── src/
│   │   ├── components/    # Reusable UI components
│   │   ├── pages/         # Feature pages
│   │   ├── services/      # API calls
│   │   └── utils/         # Helper functions
│   └── public/
└── database/              # Database schemas & migrations
```

## 🔧 Development Workflow

### Git Workflow
```bash
# Create feature branch
git checkout -b feature/mentorship-system

# Make changes and commit
git add .
git commit -m "feat: add mentor profile creation"

# Push and create PR
git push origin feature/mentorship-system
```

### Environment Setup
Create `.env` files in both `backend/` and `frontend/` directories:

**Backend (.env)**
```env
PORT=5000
MONGODB_URI=mongodb://localhost:27017/campusconnect
JWT_SECRET=your-super-secret-jwt-key
NODE_ENV=development
```

**Frontend (.env)**
```env
REACT_APP_API_URL=http://localhost:5000/api
REACT_APP_SOCKET_URL=http://localhost:5000
```

## 📊 Feature Development Status

### ✅ Completed
- [x] Basic HTML/CSS frontend structure
- [x] Navigation and routing setup
- [x] Authentication UI (signup/signin forms)
- [x] Branding and styling (CampusConnect theme)

### 🚧 In Progress
- [ ] Backend API setup
- [ ] Database schema design
- [ ] User authentication system

### 📋 Planned Features

#### 1. Seniors' Guidance & Mentorship
- [ ] User role management (Freshman/Senior/Alumni)
- [ ] Mentor profile creation and search
- [ ] Q&A system with upvoting
- [ ] Scheduling system for mentorship sessions
- [ ] Recommendation algorithm based on interests

#### 2. Events & Opportunities Board
- [ ] CRUD operations for events
- [ ] Event filtering and search
- [ ] Registration and attendance tracking
- [ ] Event categories and tags
- [ ] Calendar integration

#### 3. Skill Swap + Teammates Finder
- [ ] User skill profiles
- [ ] Matching algorithm
- [ ] Team formation system
- [ ] Project collaboration tools
- [ ] Skill verification system

#### 4. Anonymous Chat
- [ ] Real-time messaging (Socket.io)
- [ ] Anonymous user management
- [ ] Content moderation system
- [ ] Report and flagging system
- [ ] Chat room management

## 🧪 Testing

### Backend Testing
```bash
cd backend
npm test
```

### Frontend Testing
```bash
cd frontend
npm test
```

### API Testing with Postman
Import the `CampusConnect.postman_collection.json` file into Postman for pre-configured API endpoints.

## 🚀 Deployment

### Backend Deployment (Render)
1. Connect GitHub repository to Render
2. Set environment variables
3. Deploy with Node.js build command: `npm start`

### Frontend Deployment (Vercel)
1. Connect GitHub repository to Vercel
2. Set build command: `npm run build`
3. Deploy automatically on push to main branch

## 👥 Contributing

See [CONTRIBUTING.md](./CONTRIBUTING.md) for detailed contribution guidelines.

### Team Roles
- **Backend Developer**: API development, database design
- **Frontend Developer**: UI/UX implementation, state management
- **DevOps**: Deployment, CI/CD setup
- **QA Tester**: Testing, bug reporting

## 📞 Support

For questions or issues:
- Create an issue in the GitHub repository
- Contact the development team
- Check the documentation in `/docs` folder

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

**Built with ❤️ by students, for students**

