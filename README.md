# Fish Encyclopedia AI

## Project Overview

The Fish Encyclopedia AI is a web-based application designed to upload and store images and details of fish species. It automatically generates scientific descriptions for each fish entry and organizes the information alphabetically, similar to an encyclopedia. Users can upload images, scientific names, and other details through the interface, and the backend verifies and stores the information using Google Cloud.

### Features:
- Upload fish images and scientific names
- Automatically generate and store fish descriptions using AI (ChatGPT or Perplexity)
- Images and data stored securely in Google Cloud Storage
- Front-end developed in React, designed using Figma
- Python Flask-based backend for handling file uploads and API requests

## Technologies Used

- **Figma**: Used for designing the user interface
- **React**: Front-end framework for building the user interface
- **Flask**: Backend framework (Python) for handling API requests
- **Google Cloud Storage**: For storing fish images and associated data
- **Python**: Backend programming language
- **Axios/Fetch API**: For making API requests from the front-end to the backend

## Project Structure

```plaintext
Fish-Encyclopedia-AI/
│
├── frontend/                      # React frontend code
│   ├── src/                       # Source code for React components
│   └── public/                    # Public assets for the React app
│
├── backend/                       # Python Flask backend
│   ├── app.py                     # Main Flask application
│   ├── requirements.txt           # Python dependencies
│   └── credentials.json           # Google Cloud credentials (ensure this is added to .gitignore)
│
└── README.md                      # Project documentation (this file)

Installation

Prerequisites:

1. Node.js and npm: For running the React front-end.


2. Python 3.x: For running the Flask back-end.


3. Google Cloud Account: For cloud storage setup.



Backend Setup (Python)

1. Clone the repository:

git clone https://github.com/yourusername/Fish-Encyclopedia-AI.git
cd Fish-Encyclopedia-AI/backend


2. Install Python dependencies:

pip install -r requirements.txt


3. Set up Google Cloud:

Ensure your Google Cloud project and bucket are set up.

Download the credentials.json file from your Google Cloud account.

Place the credentials.json file in the backend/ directory.



4. Run the Flask app:

python app.py

The Flask app will run at http://localhost:5000.



Frontend Setup (React)

1. Navigate to the frontend directory:

cd ../frontend


2. Install dependencies:

npm install


3. Run the React development server:

npm start

The React app will run at http://localhost:3000.



API Endpoints

POST /upload: Uploads fish images to Google Cloud Storage.


Request:

POST /upload
Content-Type: multipart/form-data
Body: { file: <image_file> }

Response:

{
    "message": "File uploaded successfully",
    "file_url": "<public_url_of_file>"
}

Contributing

1. Fork the repository


2. Create a new branch (git checkout -b feature-name)


3. Commit your changes (git commit -m 'Add some feature')


4. Push to the branch (git push origin feature-name)


5. Open a pull request



License

This project is licensed under the MIT License - see the LICENSE file for details.

This `README.md` file explains the project, its structure, how to set it up, and how to use the API. You can modify it further based on your specific requirements.

