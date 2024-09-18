# Fish Encyclopedia AI

The Fish Encyclopedia AI is a web-based application that allows users to submit fish species, including images and scientific names and generates formatted information using an AI model. The data is stored in Google Sheets to avoid duplication, and the AI-generated descriptions are organized alphabetically in a Google Doc.

## Table of Contents

- [Features](#features)
- [Tech Stack](#tech-stack)
- [Installation](#installation)
- [Usage](#usage)
- [Folder Structure](#folder-structure)
- [License](#license)

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

### Prerequisites

- [Python 3.x](https://www.python.org/downloads/)
- [Node.js and npm](https://nodejs.org/en/download/)
- [Google Cloud Project](https://console.cloud.google.com/) (for API credentials)
  
### 1. Clone the Repository

```bash
git clone https://github.com/your-username/Fish-Encyclopedia-AI.git
cd Fish-Encyclopedia-AI

### 2. Backend Setup

1. Navigate to the fish-encyclopedia-backend folder:

```bash
cd fish-encyclopedia-backend
