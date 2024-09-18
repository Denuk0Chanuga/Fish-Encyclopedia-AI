y**Fish Encyclopedia AI**

The Fish Encyclopedia AI is a full-stack web application that allows users to upload scientific names and images of fish, generating detailed, AI-powered descriptions. The data is stored in Google Sheets to prevent duplicates, and the generated fish information is formatted and stored in a Google Document. The project uses React for the frontend interface and Flask for the backend, integrated with Google APIs.

Features

Fish Information Upload: Users can upload fish names and images.

Google Sheets Integration: Checks and stores fish data to avoid duplicates.

AI-Generated Descriptions: Generates scientific fish descriptions using AI models.

Google Docs Formatting: Fish information is saved and formatted in Google Docs.

React Frontend: Built using React for seamless user interactions.

Flask Backend: Manages API requests and handles data processing.



---

Table of Contents

Project Structure

Requirements

Installation

Running the Project

API Endpoints

Google API Integration



---

Project Structure

Fish-Encyclopedia-AI/
│
├── fish-encyclopedia-backend/
│   ├── app.py         # Flask app file
│   ├── service_account.json  
       # Google API service account credentials
│   ├── requirements.txt # Python dependencies
│   └── ...
│
├── fish-encyclopedia-interface/
│   ├── public/         # Public static files
│   ├── src/  # React components and frontend code
│   ├── package.json    # Node.js dependencies
│   └── ...
│
├── .gitignore
├── README.md        # Project documentation
└── ...


---

Requirements

Backend (Flask)

Python 3.8+

Flask

Flask-CORS

Google API Python Client Library


Frontend (React)

Node.js 16+

React



---

Installation

1. Clone the Repository:

First, clone the repository to your local machine:
 ``brush
git clone https://github.com/your-username/Fish-Encyclopedia-AI.git
cd Fish-Encyclopedia-AI


´´

2. Backend Setup:

Navigate to the fish-encyclopedia-backend folder and set up the Python virtual environment:

cd fish-encyclopedia-backend

Create and activate a virtual environment:

python3 -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate

Install Python dependencies:

Install the required dependencies from the requirements.txt file:

pip install -r requirements.txt

Google API Credentials:

Download the service_account.json from your Google Cloud Project and place it in the fish-encyclopedia-backend folder.

# Example: move service_account.json to backend folder
mv ~/Downloads/service_account.json ./fish-encyclopedia-backend



3. Frontend Setup:

Now, set up the React frontend by navigating to the fish-encyclopedia-interface folder:

cd ../fish-encyclopedia-interface

Install Node.js dependencies:

Install the required Node.js dependencies using the following command:

npm install


---

Running the Project

1. Start the Backend (Flask):

Make sure you're in the fish-encyclopedia-backend folder:

cd fish-encyclopedia-backend

Run the Flask app:

python app.py



2. Start the Frontend (React):

In another terminal, navigate to the fish-encyclopedia-interface folder:

cd fish-encyclopedia-interface

Start the React app:

npm start



3. Open your browser and navigate to http://localhost:3000 to interact with the Fish Encyclopedia AI interface.




---

API Endpoints

GET /api/fish
Retrieves fish data from the backend.

POST /api/fish/upload
Uploads fish names and images, generating descriptions.



---

Google API Integration

The backend integrates with Google Sheets and Google Docs via the Google API Client Libraries. Follow these steps to set up:

1. Create a Google Cloud Project and enable the Google Sheets API and Google Docs API.


2. Create a Service Account with appropriate permissions and download the credentials as service_account.json.


3. Place the service_account.json file in the fish-encyclopedia-backend folder.




---

License

This project is licensed under the MIT License - see the LICENSE file for details.


---

Contributions

Feel free to fork this repository, create a new branch, and submit pull requests for any improvements or bug fixes.


