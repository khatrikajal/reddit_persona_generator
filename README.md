
# Reddit Persona Generator

This project scrapes Reddit user/subreddit/post data, builds a user persona using the Mistral-7B model via OpenRouter, and generates a visual persona card.

##  Features

- Scrape data from Reddit user, subreddit, or post URLs using PRAW.
- Automatically extract titles, comments, subreddits, and scores.
- Generate a behavioral persona in JSON using the Mistral-7B instruct model.
- Render a high-quality persona card image using PIL.
- Works in VS Code and Jupyter environments.

##  Technologies Used

- Python
- PRAW
- OpenRouter API (Mistral-7B)
- PIL (Pillow)
- dotenv
- pandas, requests

## Installation

```bash
git clone <your-repo-url>
cd <project-folder>
pip install -r requirements.txt
```

Create a `.env` file:

```
API_KEY="your api key"
```

Download fonts:

```bash
mkdir -p fonts
wget -O fonts/Poppins-Regular.ttf https://github.com/google/fonts/raw/main/ofl/poppins/Poppins-Regular.ttf
wget -O fonts/Poppins-Bold.ttf https://github.com/google/fonts/raw/main/ofl/poppins/Poppins-Bold.ttf
```

##  Usage

1. Run the Reddit scraper script:
    - Input Reddit URL (user/subreddit/post)
    - Saves output to `scraped_reddit_data.csv`

2. Run the persona generator script:
    - Reads `scraped_reddit_data.csv`
    - Calls Mistral API
    - Generates and saves `persona_card.png`

##  Project Structure

```
project/
├── scraper.py
├── generate_persona.py
├── fonts/
│   ├── Poppins-Regular.ttf
│   └── Poppins-Bold.ttf
├── .env
├── scraped_reddit_data.csv
├── persona_card.png
├── requirements.txt
├── README.md
└── README.txt
```

##  Deliverables

- `scraped_reddit_data.csv`
- `persona_card.png`
- `README.md` / `README.txt`
- Codebase in GitHub repo

##  Tested On

- Jupyter Notebook (VS Code + Google Colab)
- Python 3.9+

##  Contact

Kajal Khatri  
kajalkhatri9373@gmail.com  
Nashik, Maharashtra  
[GitHub](https://github.com/khatrikajal/reddit_persona_generator)
