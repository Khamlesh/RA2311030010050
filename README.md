# RA2311030010050

# 📢 Campus Notification System (Frontend)

This project is a frontend application built using **React.js** for displaying campus notifications such as events, results, and placement updates. It integrates with a secure backend API and follows all evaluation requirements.

---

## 🚀 Features

* 🔐 Authentication using API (JWT Token)
* 📋 View all notifications with pagination
* ⭐ Priority notifications (Placement > Result > Event)
* 🔍 Filter notifications by type
* 📌 Read / Unread status handling
* 📱 Responsive UI (mobile + desktop)
* ⚡ Clean and minimal UI using Material UI
* 🧾 Logging middleware integration

---

## 🛠️ Tech Stack

* React.js
* JavaScript
* Material UI
* REST API (Fetch)

---

## 📂 Project Structure

```
RA2311030010050/
├── notification_app_fe/
│   ├── src/
│   ├── public/
│   ├── package.json
│
├── logging middleware/
├── notification_system_design.md
├── README.md
```

---

## 🔐 Environment Variables

Create a `.env` file inside `notification_app_fe/`:

```
REACT_APP_EMAIL=kb1311@srmist.edu.in
REACT_APP_NAME=b khamlesh gupta
REACT_APP_ROLLNO=ra2311030010050
REACT_APP_ACCESS_CODE=QkbpxH
REACT_APP_CLIENT_ID=8100f4e5-6ff0-425b-b0c8-0aa871996038
REACT_APP_CLIENT_SECRET=********
REACT_APP_API_BASE_URL=http://20.207.122.201/evaluation-service
```

---

## ⚙️ Installation & Setup

1. Clone the repository:

```
git clone https://github.com/Khamlesh/RA2311030010050.git
```

2. Navigate to frontend:

```
cd notification_app_fe
```

3. Install dependencies:

```
npm install
```

4. Start the application:

```
npm start
```

App will run at:

```
http://localhost:3000
```

---

## 🔌 API Integration

### Authentication API

```
POST /evaluation-service/auth
```

* Generates access token
* Stored in localStorage

---

### Notifications API

```
GET /evaluation-service/notifications
```

Headers:

```
Authorization: Bearer <token>
```

---

## ⭐ Priority Logic

Notifications are sorted using:

* Placement → Highest Priority
* Result → Medium Priority
* Event → Lowest Priority

Sorting order:

1. Priority
2. Latest timestamp

---

## 🧾 Logging Middleware

Custom logging function:

```
Log(stack, level, package, message)
```

Used for:

* API calls
* Errors
* User actions

---

## ⚠️ Important Notes

* Do NOT push `.env`, `node_modules`, or `build` folder
* Always fetch data from API (no hardcoding)
* Follow clean code practices

---

## 👨‍💻 Author

**B Khamlesh Gupta**
Roll No: RA2311030010050

---

## ✅ Status

✔ Completed
✔ Ready for evaluation
