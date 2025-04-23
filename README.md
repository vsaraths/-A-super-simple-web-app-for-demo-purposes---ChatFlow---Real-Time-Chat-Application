# ChatFlow - Real-Time Chat Application

A modern, real-time chat application built with React, Socket.IO, Node.js, and Redis. ChatFlow enables users to join chat rooms and communicate instantly with others in a beautiful, responsive interface.

![ChatFlow Screenshot](https://images.pexels.com/photos/7014761/pexels-photo-7014761.jpeg)

## Features

- 🚀 Real-time messaging with instant delivery
- 🏠 Multiple chat rooms with create/join functionality
- 👥 User presence indicators and typing notifications
- 💾 Message persistence with Redis (with in-memory fallback)
- 🎨 Beautiful, responsive design with smooth animations
- 🔒 Simple username-based authentication
- 📱 Works seamlessly across all devices
- 🕒 Message timestamps and history
- 🎯 Room-specific user lists

## Tech Stack

- **Frontend**:
  - React 18 with TypeScript
  - Tailwind CSS for styling
  - Socket.IO client for real-time communication
  - Lucide React for icons

- **Backend**:
  - Node.js with Express
  - Socket.IO for WebSocket connections
  - Redis for message persistence
  - CORS for cross-origin support

## Getting Started

### Prerequisites

- Node.js (v18 or higher)
- Redis server (optional, falls back to in-memory storage)

### Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/chatflow.git
   cd chatflow
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

3. Start the development servers:
   ```bash
   npm run dev:all
   ```

The application will start on `http://localhost:5173` with the backend server running on port 3001.

## Environment Variables

The following environment variables can be configured:

- `REDIS_HOST` - Redis server host (default: localhost)
- `REDIS_PORT` - Redis server port (default: 6379)
- `REDIS_PASSWORD` - Redis server password (if required)
- `PORT` - Backend server port (default: 3001)

## Project Structure

```
chatflow/
├── src/                    # Frontend source files
│   ├── components/        # React components
│   ├── context/          # React context providers
│   └── chat.css          # Custom CSS animations
├── server/                # Backend source files
│   ├── index.js          # Main server file
│   └── redis.js          # Redis configuration
└── public/               # Static assets
```

## Features in Detail

### Real-time Communication
- Instant message delivery using WebSocket connections
- Typing indicators show when users are composing messages
- User presence updates when joining/leaving rooms

### Chat Rooms
- Default rooms: General, Tech, and Random
- Create custom rooms with unique names
- Join existing rooms with live user count
- View active users in each room

### Message Persistence
- Messages are stored in Redis (or in-memory if Redis is unavailable)
- Automatic message history loading when joining rooms
- Limited to last 100 messages per room for performance

### User Experience
- Clean, modern interface with purple gradient theme
- Smooth animations for message delivery
- Responsive design works on all screen sizes
- Clear visual hierarchy and intuitive navigation

## Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

- [Socket.IO](https://socket.io/) for real-time communication
- [Redis](https://redis.io/) for message persistence
- [Tailwind CSS](https://tailwindcss.com/) for styling
- [Lucide](https://lucide.dev/) for beautiful icons