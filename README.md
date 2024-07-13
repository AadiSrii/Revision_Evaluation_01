# Revision_Evaluation_01

This project is a full-stack single-page application (SPA) that showcases detailed information about countries based on currency codes. The application utilizes React on the frontend and Node.js with Express on the backend.

# Features
User authentication (registration and login)
Fetching country details by currency code
Storing and retrieving favorite countries
Storing and retrieving search history

# Folder Structure
backend/  
├── controllers/
├── middleware/
├── models/
├── routes/
├── .env              # Environment variables (PORT, MONGO_URI, JWT_SECRET)
├── package.json      # Backend dependencies and scripts
└── server.js         # Express server setup

frontend/
├── public/
│   └── index.html    # HTML template
├── src/
│   ├── assets/       # Images, icons, etc.
│   ├── components/   # React components
│   ├── contexts/     # React context providers
│   ├── pages/        # Main pages (Home, Favorites)
│   ├── services/     # API service functions (axios)
│   ├── utils/        # Utility functions
│   ├── App.css       # Global styles
│   ├── App.js        # Main application component
│   ├── index.css     # Global CSS
│   └── index.js      # React application entry point
├── .env              # Environment variables (REACT_APP_API_URL)
├── package.json      # Frontend dependencies and scripts
Backend Setup

# Clone the repository:
git clone https://github.com/AadiSrii/Revision_Evaluation.git
cd your-repo/backend
Install dependencies:
npm install

# Set up environment variables:

Create a .env file in the backend directory with the following variables:

PORT=5000
MONGO_URImongodb+srv://aadi:Evaluation01@cluster0.1lmmpkd.mongodb.net/?retryWrites=true&w=majority&appName=Cluster0
JWT_SECRET=your_jwt_secret

# Run the server:

node index.js
The server should start running on http://localhost:5000.

Frontend Setup
Navigate to the frontend directory:

cd ../frontend
Install dependencies:

npm install
Set up environment variables:

Create a .env file in the frontend directory with the following variable:

REACT_APP_API_URL=http://localhost:5000/api
This variable specifies the base URL for API requests.

# Start the development server:

npm start
The frontend development server should start running on http://localhost:3000.

# Usage
Register/Login: Access the frontend application (http://localhost:3000) to register a new user or login with existing credentials.
Search by Currency Code: Enter a currency code in the search field to fetch and display details about countries using that currency.
Favorites: Mark countries as favorites to view them later on the Favorites page.
Search History: View your recent search history on the homepage.
# Notes
Ensure MongoDB is running locally or update MONGO_URI in .env with your MongoDB connection string.
Adjust CORS settings if deploying frontend and backend on different origins in production.
