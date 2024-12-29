# Private_Room

A responsive, real-time chat application built using HTML, Tailwind CSS, JavaScript, and Vite, designed for seamless communication within small groups.

## Live Link
Access the live application here: [Chat App](https://peaceful-beijinho-a14e69.netlify.app/)

---

## Overview
This application allows users to create or join private chat rooms, with a strict limit of four members per room. It ensures secure access through passkey validation and provides a clean and intuitive user interface for messaging.

---

## Core Features

### 1. Room Management:
- **Create New Rooms**: Users can create private rooms with custom names.
- **Join Existing Rooms**: Enter a room using its unique room ID.
- **Member Limit**: Each room supports up to 4 members.
- **Passkey Protection**: Rooms can be protected with a passkey/password for secure access.

### 2. User Interface:
- **Three Main Views**:
  - Join Room
  - Create Room
  - Chat Interface
- **Member Count Display**: Shows the current number of members in the room (e.g., 2/4).
- **Room ID Visibility**: Displays the room ID within the chat view.
- **Message History**: Chat history is scrollable for easy navigation.
- **Clear Input Area**: The message input area remains clear after sending a message.
- **Message Design**: Clear visual distinction between sent and received messages.

### 3. Authentication:
- **Passkey Validation**: Ensures only authorized users can join.
- **Username Requirement**: Users must enter a unique username to join.
- **Error Handling**: Provides feedback for invalid passkeys or full rooms.

### 4. Chat Functionality:
- **Real-Time Messaging**: Messages update instantly for all participants.
- **Message Format**:
  - Sender Name
  - Message Content
  - Timestamp
- **Readable Design**: Messages are visually organized for easy reading.

---

## Technical Requirements

### 1. Frontend Stack:
- **React with Hooks**: Utilized `useState` and `useEffect` for state management.
- **shadcn/ui Components**: Includes:
  - `Card`, `CardContent`, `CardHeader`, `CardTitle`
  - `Input`
  - `Button`
  - `Alert`
- **Lucide React Icons**: Enhances UI aesthetics with modern icons.
- **Responsive Design**: Ensures the app works seamlessly across devices.

---

## State Management
- **Room State**: Tracks whether the user is joining, creating, or chatting.
- **Room Information**:
  - Room ID
  - Passkey
  - Members
  - Messages
- **User Details**: Maintains the current user's username and status.
- **Message Input**: Tracks the content of the message being typed.
- **Error State**: Handles errors such as incorrect passkeys or room over-capacity.

---

## Getting Started

### Prerequisites
- Node.js (v14 or higher)
- Vite

### Installation
1. Clone the repository:
   ```bash
   git clone <repository-url>
   ```
2. Navigate to the project directory:
   ```bash
   cd chat-app
   ```
3. Install dependencies:
   ```bash
   npm install
   ```
4. Start the development server:
   ```bash
   npm run dev
   ```
5. Open the application in your browser at `http://localhost:3000`.

---

## Project Structure
```plaintext
├── public          # Static assets
├── src
│   ├── components  # Reusable React components
│   ├── pages       # Application views (Join, Create, Chat)
│   ├── styles      # Tailwind CSS configurations
│   ├── utils       # Utility functions
│   └── App.jsx     # Main application entry point
├── index.html      # Entry HTML file
├── tailwind.config.js # Tailwind CSS configuration
└── vite.config.js  # Vite configuration
```

---

## Technologies Used
- **HTML**: Structure of the application.
- **Tailwind CSS**: Styling framework for a responsive design.
- **JavaScript**: Core programming language for interactivity.
- **Vite**: Fast development server and build tool.

---

## Future Enhancements
- Add support for media sharing (images, videos).
- Implement typing indicators.
- Enhance error handling with custom alerts.
- Introduce themes for customizable user experience.


---

## Contributions
Contributions are welcome! Feel free to submit a pull request or open an issue to suggest improvements.

