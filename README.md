CurrentAI Application

Overview

CurrentAI is an AI-based chat application that allows users to interact with an AI model with real-time information. It includes functionality for user sign-up, login, password recovery, and conversation history management. Users can save and export their chat history once logged in. Developed a real-time conversational AI platform using Streamlit, LangChain, and TiDB Serverless, enabling users to interact with a large language model for information and tasks.

Live page link: CurrentAI Live Page

Features

Sign Up: Register a new account.
Log In: Access your account.
Forgot Password: Reset your password.
Chat: Interact with the AI.
Save Conversation: Save chat history.
Export Conversation: Download conversation history as a CSV file.
Setup Instructions
Follow these steps to set up and run the application:

Clone the Repository

git clone https://github.com/sandeepnayak123/CurrentAI.git

cd CurrentAI
Create Conda Environment

conda create --prefix ./venv python==3.10 -y
Activate the Environment

conda activate venv/
Install Required Libraries

pip install -r requirements.txt
Set Up Environment Variables, Particularly for TiDB and Google Gemini Create a .env file in the root directory of the project with the following content:

DB_HOST=something.aws.tidbcloud.com
DB_USER=something.root
DB_PASSWORD=something
DB_PORT=4000
DB_NAME=test
GOOGLE_API_KEY=something
Run the Application

streamlit run app.py
Additional Notes

Make sure to replace the placeholder values in the .env file with your actual database and API credentials.
For more details on how to use the application, refer to the in-app help and documentation.

License

This project is licensed under the MIT License - see the LICENSE file for details.
