

# 🗨️ **ChatApp**  
A **real-time chat application** with authentication, messaging, friend requests, notifications, and group chats.  

## 🚀 **Features**  
✅ **Real-time messaging** using **Socket.io**  
✅ **User authentication** with **JWT**  
✅ **Friend requests** & **notifications**  
✅ **Group chats** (create, join, manage members)  
✅ **Image & file uploads** via **Cloudinary**  
✅ **RESTful API** built with **Node.js & Express**  
✅ **MongoDB & Mongoose** for database management  

---

## 🛠️ **Tech Stack**  
### **Backend:**  
- **Node.js** with **Express.js**  
- **MongoDB** with **Mongoose**  
- **JWT authentication** for security  
- **Cloudinary** for media storage  
- **Socket.io** for real-time messaging  

### **Frontend:**  
- **React.js** with **Vite**  
- **Material-UI (MUI)** for UI components  
- **Redux Toolkit** for state management  
- **Socket.io-client** for real-time updates  
- **Axios** for API requests  

---

## 📂 **Project Setup**  

### 🏗️ **1. Clone the Repository**  
```sh
git clone https://github.com/rajakerkar/ChatApp.git
cd ChatApp
```

### ⚙️ **2. Install Dependencies**  

#### **Backend (Server)**
```sh
cd server
npm install
```

#### **Frontend (Client)**
```sh
cd client
npm install
```

### 🛠️ **3. Configure Environment Variables**  
Create a `.env` file inside the **server** directory and add:  
```env
MONGO_URI=mongodb://127.0.0.1:27017/ChatApp
JWT_SECRET=your_jwt_secret
ADMIN_SECRET_KEY=your_admin_key
NODE_ENV=DEVELOPMENT
CLIENT_URL=your_frontend_url

CLOUDINARY_CLOUD_NAME=your_cloudinary_name
CLOUDINARY_API_KEY=your_cloudinary_api_key
CLOUDINARY_API_SECRET=your_cloudinary_api_secret
```
> **⚠️ Note:** Never share your `.env` file publicly.

### 🚀 **4. Run the Application**  

#### **Start Backend**
```sh
cd server
npm start  # Runs with Nodemon
```

#### **Start Frontend**
```sh
cd client
npm run dev
```

### 🔗 **5. Open in Browser**  
Frontend: **[http://localhost:5173](http://localhost:5173)**  
Backend: **[http://localhost:5000](http://localhost:5000) (or your assigned port)**  

---

## 📜 **API Endpoints**  

### 🛠️ **User Authentication & Profile**  
| Method | Endpoint         | Description |
|--------|-----------------|-------------|
| `POST` | `/api/v1/user/new` | Register a new user |
| `POST` | `/api/v1/user/login` | User login |
| `GET` | `/api/v1/user/me` | Get logged-in user profile |
| `GET` | `/api/v1/user/logout` | Logout user |

### 🤝 **Friend Requests & Notifications**  
| Method | Endpoint         | Description |
|--------|-----------------|-------------|
| `GET` | `/api/v1/user/search` | Search for users |
| `PUT` | `/api/v1/user/sendrequest` | Send a friend request |
| `PUT` | `/api/v1/user/acceptrequest` | Accept a friend request |
| `GET` | `/api/v1/user/notifications` | Get user notifications |
| `GET` | `/api/v1/user/friends` | Get list of friends |

---

### 💬 **Chat & Group Chat Management**  
| Method | Endpoint         | Description |
|--------|-----------------|-------------|
| `POST` | `/api/v1/chat/new` | Create a new group chat |
| `GET` | `/api/v1/chat/my` | Get all user chats |
| `GET` | `/api/v1/chat/my/groups` | Get all group chats |
| `PUT` | `/api/v1/chat/addmembers` | Add members to a group |
| `PUT` | `/api/v1/chat/removemember` | Remove members from a group |
| `DELETE` | `/api/v1/chat/leave/:id` | Leave a group chat |

---

### 📩 **Messaging & Attachments**  
| Method | Endpoint         | Description |
|--------|-----------------|-------------|
| `POST` | `/api/v1/chat/message` | Send a message (with attachments) |
| `GET` | `/api/v1/chat/message/:id` | Get messages for a chat |

---

### 🔧 **Chat Management (Rename, Delete, Get Details)**  
| Method | Endpoint         | Description |
|--------|-----------------|-------------|
| `GET` | `/api/v1/chat/:id` | Get chat details |
| `PUT` | `/api/v1/chat/:id` | Rename a group |
| `DELETE` | `/api/v1/chat/:id` | Delete a chat |

---

## 👨‍💻 **Contributing**  
Want to improve this project? Follow these steps:  
1. **Fork the repository**  
2. **Create a new branch** (`git checkout -b feature-branch`)  
3. **Commit your changes** (`git commit -m "Added a new feature"`)  
4. **Push to your branch** (`git push origin feature-branch`)  
5. **Open a Pull Request**  

---

## 📄 **License**  
This project is licensed under the **MIT License**.  

## ⭐ **Show Your Support**  
If you like this project, **give it a star ⭐** on GitHub!  

---
