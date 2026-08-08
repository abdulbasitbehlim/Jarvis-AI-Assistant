# Jarvis - AI Voice Assistant

A simple voice-controlled AI assistant inspired by **Jarvis** (from Iron Man) and Alexa.

This project can listen to your voice commands, open websites, play music, fetch latest news, and answer general questions using OpenAI's GPT model.

## Features

- **Voice Recognition** – Listens for the wake word **"Jarvis"**
- **Text-to-Speech** – Speaks responses using `gTTS` + `pygame`
- **Open Websites** – Google, YouTube, Facebook, LinkedIn
- **Play Music** – Plays songs from a predefined music library (YouTube links)
- **News Headlines** – Fetches top news from India using NewsAPI
- **AI Responses** – Answers general questions using OpenAI GPT-3.5

## Project Structure

```
Jarvis-AI-Assistant/
├── main.py              # Main application
├── client.py            # Simple OpenAI test script
├── musicLibrary.py      # Music links dictionary
├── README.md            # Project documentation
├── LICENSE              # MIT License
├── .gitignore           # Git ignore rules
└── requirements.txt     # Python dependencies
```

## Requirements

- Python 3.8 or higher
- Microphone access
- Internet connection
- OpenAI API Key
- NewsAPI Key

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/abdulbasitbehlim/Jarvis-AI-Assistant.git
   cd Jarvis-AI-Assistant
   ```

2. Install the required packages:
   ```bash
   pip install -r requirements.txt
   ```

3. Get your API keys:
   - **OpenAI API Key** → [https://platform.openai.com](https://platform.openai.com)
   - **NewsAPI Key** → [https://newsapi.org](https://newsapi.org)

4. Open `main.py` and replace the placeholders:
   ```python
   newsapi = "<Your Key Here>"
   api_key = "<Your Key Here>"   # inside aiProcess function
   ```

## How to Run

```bash
python main.py
```

### How to use:
1. The assistant will say **"Initializing Jarvis...."**
2. Say the wake word: **"Jarvis"**
3. Jarvis will reply **"Ya"**
4. Give your command, for example:
   - "Open Google"
   - "Open YouTube"
   - "Play stealth"
   - "News"
   - "What is artificial intelligence?"

## Available Commands

| Command              | Action                          |
|----------------------|---------------------------------|
| Open Google          | Opens Google                    |
| Open YouTube         | Opens YouTube                   |
| Open Facebook        | Opens Facebook                  |
| Open LinkedIn        | Opens LinkedIn                  |
| Play [song name]     | Plays song from music library   |
| News                 | Speaks top news headlines       |
| Any other question   | Answers using OpenAI            |

## Music Library

You can add more songs in `musicLibrary.py`:

```python
music = {
    "stealth": "https://www.youtube.com/watch?v=...",
    "march": "https://www.youtube.com/watch?v=...",
    # Add more songs here
}
```

## Notes

- Make sure your microphone is working and permission is granted.
- The first time you run, it may take a few seconds to initialize.
- Keep your API keys private. Do **not** upload them to GitHub.

## Contributing

Feel free to fork this repository, improve the code, or add new features!

## License

This project is licensed under the **MIT License** - see the [LICENSE](LICENSE) file for details.
