It looks like you're asking for two `README.md` files, likely one for the frontend (`fish-encyclopedia-interface`) and one for the backend (`fish-encyclopedia-backend`). Below are the two separate `README.md` files for each part of the project:

### 1. `README.md` for the Frontend (`fish-encyclopedia-interface`):

```md
# Fish Encyclopedia Interface

This is the frontend application for the **Fish Encyclopedia AI** project. It is built using React and serves as the user interface where users can upload fish images and scientific names.

## Features

- Upload fish images and scientific names.
- Interact with the backend API for data storage and verification.
- Display AI-generated fish descriptions.

## Tech Stack

- **Frontend**: React.js, HTML, CSS, JavaScript
- **Backend**: Flask (Python)
- **API**: Fetch API to communicate with Flask backend

## Installation

### Prerequisites

- [Node.js and npm](https://nodejs.org/en/download/)

### 1. Clone the Repository

```bash
git clone https://github.com/your-username/Fish-Encyclopedia-AI.git
cd Fish-Encyclopedia-AI/fish-encyclopedia-interface
```

### 2. Install Node.js Dependencies

```bash
npm install
```

### 3. Start the Development Server

```bash
npm start
```

The app will be running at `http://localhost:3000`.

## Project Structure

```
fish-encyclopedia-interface/
├── public/                     # Public assets
├── src/                        # React components
│   ├── App.js                  # Main React app
│   └── components/             # UI Components
├── package.json                # Node.js dependencies
├── package-lock.json           # Locked versions of dependencies
└── README.md                   # Project documentation
```

## Usage

1. **Submit Fish Data**: Use the interface to upload fish details.
2. **View AI-Generated Descriptions**: Once uploaded, the AI will generate a fish description.

## License

This project is licensed under the MIT License.
```

### 2. `README.md` for the Backend (`fish-encyclopedia-back

Here’s the `README.md` file split into **two parts** as you requested:

---

### **Part 1: Project Overview and Setup**

```md
# Fish Encyclopedia AI

The Fish Encyclopedia AI is a web-based application that allows users to submit fish species, including images and scientific names, and generates formatted information using an AI model. The data is stored in Google Sheets to avoid duplication, and the AI-generated descriptions are organized alphabetically in a Google Doc.

## Table of Contents

- [Features](#features)
- [Tech Stack](#tech-stack)
- [Installation](#installation)
- [Backend Setup](#backend-setup)
- [Frontend Setup](#frontend-setup)
- [Running the Full Application](#running-the-full-application)

## Features

- Upload fish images and scientific names via the web interface.
- Verify and store fish details in Google Sheets.
- Automatically generate alphabetically sorted descriptions in a Google Doc using AI.
- Easy-to-use React frontend with Flask backend API.

## Tech Stack

- **Frontend**: React.js, HTML, CSS, JavaScript
- **Backend**: Python (Flask), Google Sheets API, Google Docs API
- **Database**: Google Sheets
- **AI**: OpenAI GPT (or Perplexity AI)
- **Deployment**: GitHub, Docker (optional)

## Installation

### 1. Clone the Repository

```bash
git clone https://github.com/your-username/Fish-Encyclopedia-AI.git
cd Fish-Encyclopedia-AI
```

### 2. Backend Setup

1. Navigate to the `fish-encyclopedia-backend` folder:

   ```bash
   cd fish-encyclopedia-backend
   ```

2. Create and activate a virtual environment:

   ```bash
   python3 -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```

3. Install the required Python dependencies:

   ```bash
   pip install -r requirements.txt
   ```

4. Set up Google API credentials:

   - Go to your Google Cloud Console and enable the **Google Sheets API** and **Google Docs API**.
   - Download the `service_account.json` file and place it in the `fish-encyclopedia-backend` folder.

5. Set the environment variables:

   In the `.env` file in the `fish-encyclopedia-backend` folder, define the following:

   ```bash
   SERVICE_ACCOUNT_FILE=path/to/service_account.json
   SPREADSHEET_ID=your_google_sheet_id
   ```

6. Run the Flask app:

   ```bash
   flask run
   ```

---

### **Part 2: Frontend Setup and Project Usage**

```md
### 3. Frontend Setup

1. Navigate to the `fish-encyclopedia-interface` folder:

   ```bash
   cd ../fish-encyclopedia-interface
   ```

2. Install the required Node.js dependencies:

   ```bash
   npm install
   ```

3. Start the React development server:

   ```bash
   npm start
   ```

### 4. Running the Full Application

- After setting up both the backend and frontend, ensure the Flask app and React app are running.
- Visit `http://localhost:3000` in your browser to use the Fish Encyclopedia AI interface.

## Folder Structure

```
Fish-Encyclopedia-AI/
├── fish-encyclopedia-backend/      # Backend (Flask API)
│   ├── app.py                      # Main Flask app
│   ├── requirements.txt            # Python dependencies
│   ├── .env                        # Environment variables (Google API)
│   └── service_account.json         # Google service account file
├── fish-encyclopedia-interface/     # Frontend (React)
│   ├── public/                     # Public assets
│   ├── src/                        # React components
│   ├── package.json                # Node.js dependencies
│   └── README.md                   # Frontend README
└── README.md                       # Project README
```

## Usage

1. **Uploading Fish Information**: Use the web interface to upload fish details (name, image).
2. **Verifying and Storing Data**: The backend verifies the input and stores the details in Google Sheets.
3. **Generating Fish Encyclopedia**: The AI generates the fish description and saves it in a Google Doc, organized alphabetically.

## License

This project is licensed under the MIT License.
```

---

Now the **first part** covers the overview, features, tech stack, and backend setup, while the **second part** covers the frontend setup, project folder structure, usage instructions, and the license information.
