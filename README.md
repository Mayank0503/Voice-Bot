
Voice-Activated AI Chatbot
===========================

Overview:
---------
This is a Python-based voice-activated AI chatbot that uses voice recognition and text-to-speech
to interact with users. It supports natural conversation, system control, Wikipedia search,
website opening, note writing, and more — all through your voice commands.

----------------------------------------
REQUIREMENTS:
----------------------------------------
Python version: 3.8 or above

Libraries used:
- speech_recognition : For capturing voice input and converting to text
- pyttsx3             : For speaking responses
- wikipedia-api       : For fetching Wikipedia summaries
- webbrowser          : To open websites
- datetime, time, os, subprocess, ctypes : For system-related commands
- winsound (Windows only): To beep before listening
- difflib             : For fuzzy matching similar commands

Installation:
-------------
1. Create a virtual environment (optional but recommended):
   > python -m venv chatbot_env
   > chatbot_env\Scripts\activate   (Windows)
   > source chatbot_env/bin/activate  (Linux/Mac)

2. Install required libraries:
   > pip install speechrecognition pyttsx3 wikipedia-api pyaudio

   Note: On some systems, you may need to install `pyaudio` using a .whl file if direct install fails.

3. Run the bot:
   > python voice_bot.py

----------------------------------------
USAGE:
----------------------------------------

When you run the bot, it will greet you based on the time of day and start listening for commands.

You will hear a beep indicating it's ready for your input.

Example Voice Commands You Can Say:
-----------------------------------
- "open github"
- "open stack overflow"
- "search Wikipedia for Alan Turing"
- "what is the time"
- "how are you"
- "hello"
- "write a note"
- "shutdown" (requires admin rights)
- "restart"
- "lock the system"
- "exit" or "quit" (to stop the bot)

Smart Recognition:
------------------
- The bot uses fuzzy matching to understand variations like:
    "how are u", "how r you", "how ru" → all are understood as "how are you"

- You do NOT have to be exact with phrasing. The bot is trained to understand the intent.

----------------------------------------
NOTES:
----------------------------------------
- Ensure your microphone is working.
- Run VS Code as Administrator if using shutdown/restart/lock commands on Windows.
- Works best in quiet environments.
- Works only on Windows by default (due to `winsound`); cross-platform support can be added.

Support:
--------
You can expand it to include:
- Wake-word detection
- Multi-language support
- GUI with Tkinter
- Personalized greetings
- Reminders or calendar integrations

Let me know if you'd like help extending the project further.
