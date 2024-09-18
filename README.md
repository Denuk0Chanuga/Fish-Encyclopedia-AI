
***Fish Encyclopedia AI***

A web-based Fish Encyclopedia that allows users to upload fish photos, enter scientific details, and store them in a Google Sheet. The system generates detailed scientific descriptions using AI and organizes the fish details alphabetically in a Google Doc.

Project Structure

Fish-Encyclopedia-AI/
│
├── fish-encyclopedia-backend/     # Flask backend directory
│   ├── app.py                     # Main Flask app file
│   ├── service_account.json        # Google API service account file
│   ├── requirements.txt            # Python dependencies
│   └── utils/                      # Backend utility functions
│       ├── gsheet_handler.py       # Google Sheets integration
│       └── gdoc_handler.py         # Google Docs integration
│
├── fish-encyclopedia-interface/    # React frontend directory
│   ├── public/                     # Public files
│   ├── src/                        # React source code
│   ├── package.json                # Frontend dependencies
│   └── .env                        # Environment variables for API keys
│
└── README.md                       # Project documentation

Prerequisites

Before running this project, make sure you have the following installed:

Python 3.x

Node.js (for React)

Flask (for backend)

Google API service account (for Sheets and Docs integration)

React (for frontend)


Backend Setup (Flask)

1. Navigate to the Backend Directory:

cd fish-encyclopedia-backend


2. Create a Virtual Environment:

python -m venv venv
source venv/bin/activate   # For Windows use `venv\Scripts\activate`


3. Install Dependencies:

pip install -r requirements.txt


4. Set Up Environment Variables:

Ensure that SERVICE_ACCOUNT_FILE and SPREADSHEET_ID are set up properly in the .env file.


5. Run the Flask App:

python app.py


6. API Endpoints:

GET /api/fish - Fetches fish data from Google Sheets.

POST /api/fish - Uploads fish details and photo to the system and updates the Google Sheet.




Frontend Setup (React)

1. Navigate to the Frontend Directory:

cd fish-encyclopedia-interface


2. Install Dependencies:

npm install


3. Run the React App:

npm start

The app should now be running on http://localhost:3000.



Google Sheets & Docs Integration

1. Service Account:

Set up a Google API service account and enable Google Sheets and Google Docs APIs. Download the service_account.json file and place it in the fish-encyclopedia-backend directory.


2. Google Sheet:

Create a Google Sheet to store fish data and add the `SPREAD



