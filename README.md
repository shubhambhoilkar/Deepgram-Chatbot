**Terminal-Based Voice Chatbot with Deepgram and OpenAI**

***Overview***

This is a terminal-based voice chatbot that integrates Deepgram's real-time transcription API for capturing speech and OpenAI's GPT models for generating intelligent responses. It listens to your microphone input, transcribes the speech, and provides AI-powered replies directly in the terminal.

Features

🎧 Live speech-to-text transcription using Deepgram.

🤖 AI-powered responses using OpenAI GPT models.

⏳ Automatic silence detection with configurable timeout (default: 10 seconds).

🔄 Continuous conversation until user terminates.

🖥️ Runs seamlessly in a terminal environment (Windows).

Application Structure

project-root/
│
├── refere_deepgram.py       # Main application script
├── requirements.txt         # Python dependencies
├── .env                     # API keys and configuration
└── README.md                # Project documentation

Setup Instructions

Clone the Repository

git clone <your-repo-url>
cd <your-project-folder>

Install Dependencies
Ensure you are using Python 3.12.

pip install -r requirements.txt

Configure Environment Variables
Create a .env file in the project root:

OPENAI_API_KEY=your-openai-api-key
DEEPGRAM_API_KEY=your-deepgram-api-key

Run the Application

python refere_deepgram.py

Key Notes

The chatbot waits for user speech and allows you to speak naturally.

If silence is detected for 10 seconds, it prompts: "Are you speaking?"

Graceful termination: Use Ctrl+C to stop the application safely.

No persistent memory: Each session is stateless and does not retain previous conversations.

License

This project is created for learning as well as development purpose. 

