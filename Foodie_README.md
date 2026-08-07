# 🍽️ Foodie

Foodie is a full-stack food ordering and team meal coordination platform that integrates restaurant discovery, polling, Slack notifications, and authentication into a single application.

## ✨ Features

- 🔐 User authentication with OTP verification
- 👥 User registration approval workflow
- 🍔 Swiggy & Zomato restaurant integration
- 📋 Create scheduled and instant food polls
- 💬 Slack integration for interactive polls
- 📊 Live poll results and voting
- ⏰ Recurring poll scheduler
- 📧 Email notifications
- 🌐 REST API backend
- ⚛️ Modern React frontend built with Vite

---

## 🏗️ Tech Stack

### Frontend
- React 19
- Vite
- Tailwind CSS
- React Router
- Axios
- Ant Design
- Radix UI

### Backend
- Node.js
- Express.js
- MongoDB + Mongoose
- JWT Authentication
- Nodemailer
- Socket.IO
- Slack Bolt API
- Node Cron

### Automation
- Python scripts for launching Swiggy automation

---

## 📂 Project Structure

```text
Foodie/
├── frontend/          # React application
├── backend/           # Express API
├── python-scripts/    # Automation scripts
├── start.sh           # Startup script
└── package.json
```

---

## 🚀 Installation

### Clone

```bash
git clone https://github.com/dirwolf/Foodie.git
cd Foodie
```

### Backend

```bash
cd backend
npm install
npm start
```

### Frontend

```bash
cd frontend
npm install
npm run dev
```

---

## ⚙️ Environment Variables

Create a `.env` file inside the backend directory.

Example:

```env
PORT=8080
MONGO_URI=your_mongodb_uri
JWT_SECRET=your_secret
EMAIL_USER=your_email
EMAIL_PASS=your_password

SLACK_BOT_TOKEN=your_token
SLACK_SIGNING_SECRET=your_secret
```

---

## 🔌 Main API Endpoints

### Authentication

- POST `/register-verify`
- POST `/registration-approved`
- POST `/registration-rejected`
- POST `/login`
- POST `/send-otp`
- POST `/verify-otp`
- PUT `/update-password`

### Food APIs

- POST `/api/swiggy`
- POST `/api/zomato`
- GET `/api/restauant/swiggy`
- GET `/api/swiggy/menu`

### Poll APIs

- POST `/api/polls/create`
- POST `/api/polls/poll-start`
- POST `/api/polls/done`
- DELETE `/api/polls/delete/:pollId`

---

## 💬 Slack Integration

Foodie supports Slack interactive messages for:

- Poll creation
- Voting
- Live result viewing
- Team food coordination

---

## 📧 Email Support

The application uses Nodemailer to:

- Send OTPs
- Registration workflow emails
- Password recovery

---

## 🐍 Python Automation

Python scripts are included for automating Swiggy-related workflows.

```
python python-scripts/launch_swiggy.py
```

---

## 🛠 Development

Frontend

```bash
npm run dev
```

Backend

```bash
npm start
```

Production frontend

```bash
npm run build
```

---

## 📌 Future Improvements

- Payment integration
- Order tracking
- Restaurant recommendations
- Push notifications
- Admin dashboard analytics

---

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch
3. Commit your changes
4. Open a Pull Request

---

## 📄 License

This project is licensed under the ISC License.

---

## 👨‍💻 Author

Developed by the Foodie Team.

If you found this project useful, consider giving it a ⭐ on GitHub.
