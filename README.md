# React Chatbot Project

A simple interactive chatbot built with React and Vite that simulates conversations between a user and a robot.

## Features

- Real-time chat interface
- Auto-scrolling messages
- User and robot message distinction
- Message history preservation
- Responsive design
- Clean and modern UI

## Tech Stack

- React 18
- Vite
- CSS Modules
- supersimpledev Chatbot API

## Project Structure

```
chatbot-project/
├── src/
│   ├── assets/
│   │   ├── robot.png
│   │   └── user.png
│   ├── components/
│   │   ├── ChatInput.jsx
│   │   ├── ChatInput.css
│   │   ├── ChatMessage.jsx
│   │   ├── ChatMessage.css
│   │   ├── ChatMessages.jsx
│   │   └── ChatMessages.css
│   ├── App.jsx
│   ├── App.css
│   ├── main.jsx
│   └── index.css
├── public/
├── package.json
├── vite.config.js
└── README.md
```

## Setup and Installation

1. Clone the repository:
```bash
git clone [repository-url]
```

2. Install dependencies:
```bash
cd chatbot-project
npm install
```

3. Start the development server:
```bash
npm run dev
```

## Components

### App.jsx
- Main component that handles the state management
- Initializes chat with default messages
- Contains the layout structure

### ChatMessages.jsx
- Displays the message history
- Handles auto-scrolling to latest messages
- Maps through messages and renders individual ChatMessage components

### ChatMessage.jsx
- Renders individual message bubbles
- Handles different styles for user and robot messages
- Displays profile images for each message type

### ChatInput.jsx
- Handles user input
- Manages message sending functionality
- Integrates with the Chatbot API for responses

## Styling

- Each component has its own CSS file
- Responsive design with flexbox
- Modern UI with rounded corners and smooth transitions
- Distinct visual separation between user and robot messages

## Features in Detail

### Message Structure
Each message contains:
- message: The text content
- sender: Either 'user' or 'robot'
- id: Unique identifier

### Auto-scrolling
- Messages container automatically scrolls to the latest message
- Uses useRef and useEffect hooks for scroll management

### Input Handling
- Clear input after sending
- Prevent empty messages
- Immediate response from chatbot

## Future Improvements

1. Add typing indicators
2. Implement message timestamps
3. Add message delivery status
4. Support for multimedia messages
5. Add user authentication
6. Implement message persistence

## Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## License

This project is licensed under the MIT License - see the LICENSE file for details
