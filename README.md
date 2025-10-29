🤖 Personal-AI-Chatbot-using-Generative-AI
A beautiful, modern AI chatbot web app powered by Gemini 2.5 Flash (Google Generative AI API) and built with Flask. Features live chat, step-by-step answers, easy color customization, and a clean user interface.

✨ Features
Conversational AI: Real-time chat using Google Gemini 2.5 Flash

Step-by-step responses: Bot displays lists, steps, and formatting for clear answers

Beautiful UI: Responsive, clean chat interface based on HTML, CSS, and JS

Custom bot avatar: Use any image for your AI agent

Live typing indicator: See when the bot is thinking

Clear chat history: With one click

Dark/light color themes: Easy to change via CSS variables

Modern UX: Mobile-friendly, animated, and accessible

📁 Project Structure
text
your-chatbot-project/
├── app.py                # Flask backend (Python)
├── templates/
│   └── index.html        # Main chat UI page
├── static/
│   ├── style.css         # All custom and responsive CSS
│   └── script.js         # Frontend logic, fetches bot answers, formats replies
└── README.md             # (this file)
🚀 Getting Started
Prerequisites
Python 3.8+

A Google Gemini API key (get one here)

Internet connection (for API and CDN icons/fonts)

Install dependencies
bash
pip install flask google-generativeai
Setup your API key
The app will automatically use the key from the environment variable GOOGLE_API_KEY.
For best security, set your key like this:

Linux/macOS

bash-
export GOOGLE_API_KEY=your-key-here

Windows

text
set GOOGLE_API_KEY=your-key-here
Or edit app.py and put your key in the placeholder (not recommended for production).

Run the app
bash
python app.py
Open http://localhost:5000 in your browser.

✏️ Bot Format & Reply Features
The bot formats numbered lists, bullet points, bold/italic text, and preserves line breaks.
For best step-by-step answers, use prompts like:

"Explain XYZ in steps"

"Give me a numbered list of tips about Python"

Example Output:

text
1. First step
2. Second step
3. Third step


🐞 Troubleshooting
If chat responses do not display right, hard-refresh your browser (Ctrl+F5)

If Flask throws a "not JSON serializable" error, make sure the backend extracts plain text from the Gemini response (see /chat route in app.py)

If styles don't load, check that index.html links to /static/style.css and /static/script.js

Test your API key by running a simple Gemini test script separately

Use browser DevTools (F12) for network and console errors

📄 License
MIT — free to use, modify, and share.

🙏 Credits
Google Gemini API (https://ai.google.dev/)

Font Awesome for icons

Design inspiration from modern chatbot UIs (Dribbble, UI8, etc.)

Enjoy your personal AI assistant! 🚀
