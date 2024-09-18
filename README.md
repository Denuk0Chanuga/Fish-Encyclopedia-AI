

Installation

1. Clone the Repository:

First, clone the repository to your local machine:

git clone https://github.com/your-username/Fish-Encyclopedia-AI.git
cd Fish-Encyclopedia-AI


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

