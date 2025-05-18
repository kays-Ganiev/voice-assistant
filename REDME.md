# Voice Assistant Calendar Project

A simple voice assistant that integrates with Google Calendar, supports speech recognition, text-to-speech, and can create notes locally.

## Features

Wake word: Listens for a configurable wake phrase (hey you).

Calendar lookup: Fetches and reads aloud events from Google Calendar for specified dates.

Natural date parsing: Understands dates from phrases like "today", weekdays, and explicit days/months.

Note taking: Listens to and saves user notes as timestamped text files.

Cross-platform: Uses open on macOS; can be adapted for other OSes.

## Installation

 - Clone the repository:

```bash
git clone https://github.com/kays-Ganiev/voice-assistant.git
cd voice-assistant-calendar
```

 - Create and activate a virtual environment:

 ``` bash
 python3 -m venv venv
 ```

```bash
source venv/bin/activate    # macOS/Linux
```

```bash
venv\Scripts\activate     # Windows
```

- Install dependencies:

```bash
pip install -r requirements.txt
```

- Set up Google Calendar API credentials:

Enable the Google Calendar API in the Google Developers Console.

Download credentials.json and place it in the project root.

The first run will generate token.pickle via OAuth.

## Usage

```bash
python main.py
```

Speak the wake word (default: hey you).

Ask about your schedule:

"What do I have today?"

"Do I have plans next Monday?"

Create a note:

"Make a note"

"Remember this"

Configuration

Wake word: Modify the WAKE variable in main.py.

Speech rate: Adjust engine.setProperty('rate', ...) in speak().

## License

This project is licensed under the MIT License. See LICENSE for details.
