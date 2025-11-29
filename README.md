# AI Chatbot (Flask + OpenAI)

A simple AI Chatbot web app using Flask (backend) and a lightweight frontend.
The backend forwards user messages to the OpenAI Chat Completions API (gpt-3.5-turbo).

## Features
- Simple chat UI
- Conversation history saved in the browser session
- Easy to run locally or deploy (Dockerfile included)

## Requirements
- Python 3.8+
- An OpenAI API key (set as environment variable `OPENAI_API_KEY`)

## Quick start (local)
```bash
git clone <your-repo-url>
cd ai-chatbot
python -m venv venv
source venv/bin/activate        # macOS / Linux
venv\Scripts\activate         # Windows PowerShell
pip install -r requirements.txt
export OPENAI_API_KEY="sk-..."  # Windows: set OPENAI_API_KEY=sk-...
flask run
```
Then open http://127.0.0.1:5000

## Deploy to GitHub
1. Create a new repository on GitHub.
2. Follow the commands below to push the project.

```bash
git init
git add .
git commit -m "Initial commit: AI Chatbot"
git branch -M main
git remote add origin https://github.com/<your-username>/<repo-name>.git
git push -u origin main
```

## Notes
- This project uses the OpenAI REST API. Replace the model name if you prefer another model.
- Do **not** commit your API key to the repository. Use environment variables or GitHub Secrets for deployments.

## License
MIT
