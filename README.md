Fish Encyclopedia AI

This project aims to create a fish encyclopedia where users can upload fish images and names. The app will generate scientific descriptions of the fish, verify duplicate entries using Google Sheets, and store the generated content in a well-formatted Google Doc using AI.

Table of Contents

1. Project Structure


2. Prerequisites


3. Installation


4. Backend Setup


5. Frontend Setup


6. Running the Application


7. API Endpoints


8. Contributing



Project Structure

The project is structured into two main components:

Backend: Python Flask app, responsible for processing requests, interacting with Google Sheets, and handling AI integration.

Frontend: React app, responsible for the user interface where users can interact with the system.


Fish-Encyclopedia-AI/
│
├── fish-encyclopedia-backend/
│   ├── app.py              # Main Flask app
│   ├── requirements.txt     # Backend dependencies
│   ├── service_account.json # Google service account file (add your own credentials)
│   └── ...
├── fish-encyclopedia-interface/
│   ├── public/              # Public folder for frontend
│   ├── src/                 # Source code for React frontend
│   ├── package.json         # Frontend dependencies
│   └── ...
├── README.md
└── ...

Prerequisites

Before running the project, ensure you have the following installed on your machine:

Python 3.x

Node.js and npm

Flask (installed via pip)

React (installed via npx or npm)


You will also need a Google Cloud project with a service account to interact with Google Sheets and Google Docs.

Installation

1. Clone this repository:

git clone https://github.com/your-username/Fish-Encyclopedia-AI.git
cd Fish-Encyclopedia-AI



Backend Setup

1. Navigate to the backend directory:

cd fish-encyclopedia-backend


2. Create and activate a virtual environment:

python3 -m venv venv
source venv/bin/activate  # For Linux/MacOS
venv\Scripts\activate     # For Windows


3. Install the required dependencies:

pip install -r requirements.txt


4. Add your Google Cloud service_account.json to the fish-encyclopedia-backend/ directory. This is required for interacting with Google Sheets and Google Docs.


5. Set the environment variables:

export GOOGLE_APPLICATION_CREDENTIALS="service_account.json"


6. Run the Flask backend:

python app.py



The backend will now be running on http://localhost:5000.

Frontend Setup

1. Navigate to the frontend directory:

cd ../fish-encyclopedia-interface


2. Install the dependencies:

npm install


3. Start the React development server:

npm start



The frontend will now be running on http://localhost:3000.

Running the Application

1. Ensure both the backend and frontend servers are running. Access the app by navigating to http://localhost:3000 in your web browser.


2. The frontend communicates with the backend using API requests to submit fish data, fetch descriptions, and store data in Google Sheets and Docs.



API Endpoints

GET /api/fish
Retrieves all the fish stored in the Google Sheets.

POST /api/fish
Adds a new fish entry, generating scientific details using AI and storing the data in Google Sheets.


Example POST request body:

{
  "name": "Clownfish",
  "image_url": "https://example.com/clownfish.jpg",
  "scientific_name": "Amphiprioninae"
}

Contributing

Feel free to fork this project and submit pull requests if you wish to contribute. Any ideas, issues, or improvements are welcome.