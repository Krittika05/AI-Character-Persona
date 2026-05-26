# Persona — AI Character Studio

A beautifully designed single-page AI character chat simulator. Talk to **48 distinct AI characters** across **6 themed universes** — each with their own voice, personality, and visual identity.

## Features

- **48 unique characters** across 6 themes
  - **Classic** — Mentor, Comedian, Expert, Storyteller, Coach, Therapist, Tech Sage, Visionary
  - **Marvel Universe** — Iron Man, Captain America, Thor, Black Widow, and more
  - **Anime Heroes** — Iconic protagonists from beloved series
  - **DC Comics** — Batman, Superman, Wonder Woman, and more
  - **Studio Ghibli** — Beloved Ghibli characters
  - **Disney Characters** — Disney heroes & dreamers
- **Dual AI provider support**
  - **FREE** — Google Gemini (get a key in 30 seconds at [aistudio.google.com](https://aistudio.google.com/app/apikey))
  - **PREMIUM** — Anthropic Claude (pay-as-you-go at [console.anthropic.com](https://console.anthropic.com))
  - Auto-detects which provider from the key
- **Per-character chat history** — switch characters or themes any time, history is saved
- **Light & dark mode** — toggleable theme
- **Character profiles** — personality, specialty, voice, and example prompts
- **Bookmarkable conversations**
- **Responsive design** — works on mobile, tablet, and desktop
- **No build process** — single HTML file, pure vanilla JavaScript

## Getting Started

1. Open `index.html` in any modern browser.
2. Click the 🔑 icon and paste your AI API key (Gemini or Claude).
3. Choose a theme from the dropdown next to the logo.
4. Pick a character on the right.
5. Start chatting — or click an example prompt to begin.

```bash
# Or serve locally
python -m http.server 8766
# Then open http://localhost:8766
```

## Project Structure

```
persona/
├── index.html    # The entire app (HTML, CSS, JS in one file)
└── README.md     # This file
```

## How It Works

- **API keys** are stored locally in your browser (`localStorage`) — never sent to any server other than the AI provider you choose.
- **Conversation history** is also stored locally per character.
- The provider (Gemini vs Claude) is auto-detected from the key format.
- Each character has a hand-crafted system prompt that shapes their voice — Iron Man is sarcastic, Batman is terse, Naruto is loud, etc.

## Browser Support

Works on all modern browsers (Chrome, Firefox, Safari, Edge).

## Privacy

- No tracking, no analytics, no backend.
- Your API key and chat history never leave your browser, except for the actual chat messages sent to your chosen AI provider.

## Credits

Built as a creative exploration of single-file web apps and AI character roleplay.
