Reddit Persona Generator
========================

This tool scrapes Reddit data (user, subreddit, post), analyzes user behavior via Mistral-7B (OpenRouter), and generates a visual persona card using Python.

Features:
- Scrape Reddit activity (titles, comments, scores, subreddits)
- Extract username and persona traits
- Call OpenRouter Mistral-7B instruct model for persona JSON
- Render persona card as image with Poppins fonts

Installation:
-------------
1. Install dependencies:
   pip install -r requirements.txt

2. Create .env file with API key:
   API_KEY=your_api_key

3. Download fonts:
   mkdir -p fonts
   wget -O fonts/Poppins-Regular.ttf https://github.com/google/fonts/raw/main/ofl/poppins/Poppins-Regular.ttf
   wget -O fonts/Poppins-Bold.ttf https://github.com/google/fonts/raw/main/ofl/poppins/Poppins-Bold.ttf

Usage:
------
1. Run Reddit scraper:
   - Input Reddit URL (user, subreddit, or post)
   - Data saved to scraped_reddit_data.csv

2. Run persona generator:
   - Reads scraped_reddit_data.csv
   - Calls Mistral API and saves persona_card.png

Files:
------
- scraper.py
- generate_persona.py
- fonts/
- scraped_reddit_data.csv
- persona_card.png
- .env
- requirements.txt
- README.md
- README.txt

Created by Kajal Khatri

[GitHub](https://github.com/khatrikajal/reddit_persona_generator)