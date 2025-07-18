# ChatApp - Real-time Chat Application

A modern, real-time chat application built with React, Node.js, and Socket.IO. Features include real-time messaging, user avatars, typing indicators, and a beautiful UI with smooth animations.

## Features

- 🚀 **Real-time messaging** with Socket.IO
- 👥 **User management** with online status
- 🎨 **Beautiful UI** with modern design and animations
- 📱 **Responsive design** that works on all devices
- ⌨️ **Typing indicators** to show when users are typing
- 🖼️ **Avatar selection** with generated avatars
- ⚡ **Instant message delivery** with no page refresh
- 🎭 **Smooth animations** using Framer Motion

## Tech Stack

### Backend
- **Node.js** - JavaScript runtime
- **Express.js** - Web framework
- **Socket.IO** - Real-time communication
- **CORS** - Cross-origin resource sharing
- **UUID** - Unique identifier generation

### Frontend
- **React** - UI library
- **Styled Components** - CSS-in-JS styling
- **Framer Motion** - Animation library
- **Socket.IO Client** - Real-time client
- **React Icons** - Icon library
- **Date-fns** - Date formatting

## Prerequisites

Before running this application, make sure you have the following installed:

- **Node.js** (version 14 or higher)
- **npm** (comes with Node.js)

## Installation

1. **Clone the repository**
   ```bash
   git clone <repository-url>
   cd chatapp
   ```

2. **Install dependencies**
   ```bash
   # Install server dependencies
   npm install
   
   # Install client dependencies
   cd client
   npm install
   cd ..
   ```

   Or use the convenience script:
   ```bash
   npm run install-all
   ```

## Running the Application

### Development Mode

1. **Start both server and client simultaneously:**
   ```bash
   npm run dev
   ```

   This will start:
   - Backend server on `http://localhost:5000`
   - Frontend client on `http://localhost:3000`

2. **Or run them separately:**

   **Terminal 1 - Start the server:**
   ```bash
   npm run server
   ```

   **Terminal 2 - Start the client:**
   ```bash
   npm run client
   ```

### Production Mode

1. **Build the client:**
   ```bash
   npm run build
   ```

2. **Start the server:**
   ```bash
   npm start
   ```

## Usage

1. Open your browser and navigate to `http://localhost:3000`
2. Enter a username and select an avatar
3. Click "Join Chat" to enter the chat room
4. Start messaging with other users in real-time!

## Project Structure

```
chatapp/
├── server/
│   └── index.js          # Main server file with Socket.IO setup
├── client/
│   ├── public/
│   │   └── index.html    # Main HTML file
│   ├── src/
│   │   ├── components/
│   │   │   ├── LoginScreen.js    # User login component
│   │   │   ├── ChatRoom.js       # Main chat interface
│   │   │   ├── Message.js        # Individual message component
│   │   │   └── UserList.js       # Online users list
│   │   ├── context/
│   │   │   └── ChatContext.js    # Global state management
│   │   ├── App.js                # Main React component
│   │   └── index.js              # React entry point
│   └── package.json              # Client dependencies
├── package.json                  # Server dependencies
└── README.md                     # This file
```

## API Endpoints

- `GET /api/users` - Get all online users
- `GET /api/messages` - Get all messages

## Socket.IO Events

### Client to Server
- `join` - User joins the chat
- `sendMessage` - Send a new message
- `typing` - User typing indicator

### Server to Client
- `userJoined` - New user joined
- `newMessage` - New message received
- `userTyping` - User typing indicator
- `userLeft` - User left the chat

## Customization

### Changing the Server Port
Edit the `PORT` variable in `server/index.js` or set the `PORT` environment variable.

### Styling
The application uses Styled Components for styling. You can modify the styles in each component file.

### Avatars
The application uses DiceBear API for avatar generation. You can change the avatar URLs in `LoginScreen.js`.

## Contributing

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Test thoroughly
5. Submit a pull request

## License

This project is licensed under the MIT License.

## Support

If you encounter any issues or have questions, please open an issue on the repository.

---

**Happy Chatting! 🎉** #   c h a t a p p  
 