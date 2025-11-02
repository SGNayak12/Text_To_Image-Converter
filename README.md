# Text to Image Converter

A full-stack web application that converts textual descriptions into images using AI technology. The application features user authentication, credit system, and secure payment integration.

## Tech Stack

### Frontend (Client)
- **Framework**: React.js (v18)
- **Build Tool**: Vite
- **Routing**: React Router DOM (v6)
- **Styling**: TailwindCSS
- **Animation**: Framer Motion
- **HTTP Client**: Axios
- **Notifications**: React Toastify

### Backend (Server)
- **Runtime**: Node.js
- **Framework**: Express.js
- **Database**: MongoDB with Mongoose ODM
- **Authentication**: JSON Web Tokens (JWT) with bcrypt
- **Payment Integration**: 
  - Razorpay
  - Stripe
- **Environment Variables**: dotenv
- **Development**: Nodemon

## Project Structure

```
├── client/                 # Frontend application
│   ├── public/            # Static files
│   ├── src/
│   │   ├── assets/       # Media files and assets
│   │   ├── components/   # Reusable React components
│   │   │   ├── Description.jsx
│   │   │   ├── Footer.jsx
│   │   │   ├── GenerateBtn.jsx
│   │   │   ├── Header.jsx
│   │   │   ├── Login.jsx
│   │   │   ├── Navbar.jsx
│   │   │   ├── Steps.jsx
│   │   │   └── Testimonials.jsx
│   │   ├── context/     # React Context for state management
│   │   ├── lib/         # Utility functions and helpers
│   │   ├── pages/       # Application pages/routes
│   │   │   ├── BuyCredit.jsx
│   │   │   ├── Home.jsx
│   │   │   ├── Result.jsx
│   │   │   └── Verify.jsx
│   │   ├── App.jsx      # Main application component
│   │   └── main.jsx     # Application entry point
│   └── package.json
│
└── server/                # Backend application
    ├── configs/          # Configuration files
    │   └── mongodb.js    # Database configuration
    ├── controllers/      # Route controllers
    │   ├── imageController.js
    │   └── UserController.js
    ├── middlewares/      # Custom middleware
    │   └── auth.js       # Authentication middleware
    ├── models/           # MongoDB models
    │   ├── transactionModel.js
    │   └── userModel.js
    ├── routes/           # API routes
    │   ├── imageRoutes.js
    │   └── userRoutes.js
    ├── server.js         # Server entry point
    └── package.json

```

## Features

1. User Authentication
   - Login/Register functionality
   - JWT-based authentication
   - Secure password hashing

2. Image Generation
   - Text to image conversion
   - Result display and management

3. Credit System
   - Credit-based usage
   - Credit purchase functionality

4. Payment Integration
   - Secure payment processing
   - Multiple payment gateway support (Razorpay, Stripe)

## Getting Started

### Prerequisites
- Node.js (v14 or higher)
- MongoDB
- NPM or Yarn

### Installation

1. Clone the repository
```bash
git clone https://github.com/SGNayak12/Text_To_Image-Converter.git
cd Text_To_Image-Converter
```

2. Install frontend dependencies
```bash
cd client
npm install
```

3. Install backend dependencies
```bash
cd ../server
npm install
```

4. Set up environment variables
Create `.env` files in both client and server directories with necessary configurations.

5. Start the development servers

Frontend:
```bash
cd client
npm run dev
```

Backend:
```bash
cd server
npm run server
```

## Contributing

welcome contributions to improve the Text to Image Converter! Here's how you can help:

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

### Guidelines
- Write clean, maintainable code
- Follow existing code style and conventions
- Include comments where necessary
- Update documentation as needed
- Test your changes thoroughly



