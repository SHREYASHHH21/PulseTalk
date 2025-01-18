# **PulseTalk**

A lightweight, real-time chat application built using **Node.js**, **Express**, and **Socket.IO**. This project demonstrates the fundamentals of WebSocket-based communication for building scalable and feature-rich chat platforms.

---

## **Features**
- **Real-Time Messaging**: Users can exchange messages instantly.
- **User Management**: Tracks online users and supports one-to-one or group chats.
- **Room Support**: Users can join specific chat rooms for group conversations.
- **Typing Indicators**: Displays when other users are typing (optional).
- **Message Persistence**: Temporarily stores messages (can integrate a database like MongoDB for long-term storage).
- **Scalable Architecture**: Easily extendable for authentication, file sharing, and message history.

---

## **Tech Stack**
- **Backend**:  
  - [Node.js](https://nodejs.org/)  
  - [Express](https://expressjs.com/)  
  - [Socket.IO](https://socket.io/)  

- **Frontend**:  
  - [React.js](https://reactjs.org/) (optional, can be replaced with any frontend framework)  
  - [Socket.IO Client](https://socket.io/docs/v4/client-api/)  

- **Database (Optional)**:  
  - MongoDB

---

## **Getting Started**

### **1. Clone the Repository**
```bash
git clone https://github.com/SHREYASHHH21/PulseTalk.git
cd <repo-name>
```

### **2. Install Dependencies**
```bash
npm install
```

### **3. Configure Environment Variables**
Create a `.env` file in the root directory and add the following:
```env
PORT=5000
```

### **4. Run the Server**
```bash
npm start
```

### **5. Connect the Frontend**
(Optional) Use the provided frontend or build your own. Connect it to the server at `http://localhost:5000`.

---

## **API Endpoints**

### **Base URL**: `http://localhost:5000`

| Method | Endpoint            | Description                |
|--------|---------------------|----------------------------|
| `GET`  | `/api/messages/:id` | Fetch messages of a user   |
| `POST` | `/api/messages/send/:id` | Send a new message     |

---

## **Folder Structure**
```
/root
├── /node_modules
├── /routes
│   ├── message.routes.js
│   └── user.routes.js
├── /controllers
│   ├── message.controller.js
│   └── user.controller.js
├── /models
│   ├── message.model.js
│   └── user.model.js
├── /frontend (Optional)
│   ├── /src
│   └── /public
├── server.js
└── package.json
```

---

## **Future Enhancements**
- Add user authentication with JWT.
- Store messages in MongoDB for persistence.
- Implement group chats and file sharing.
- Add notifications for unread messages.

---

## **Contributing**
Contributions are welcome!  
1. Fork the repository.  
2. Create a feature branch: `git checkout -b my-new-feature`.  
3. Commit your changes: `git commit -m 'Add some feature'`.  
4. Push to the branch: `git push origin my-new-feature`.  
5. Submit a pull request.

---

## **License**
This project is licensed under the MIT License.

---

Feel free to fork this repository and enhance it to build your own chat platform.

