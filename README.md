# redditAuto

**redditAuto** is a Python-based automation tool currently in development. It is designed to interact with the Reddit API to assist community moderators by automating routine tasks, filtering spam, and providing real-time data lookups.

## 🚀 Project Goals

The primary objective of this project is to reduce the workload on human moderators and provide faster responses to community queries.

* **Spam Filtering:** Automated detection of spam patterns and low-quality submissions using heuristic analysis.
* **Moderation Support:** auto-flagging content that requires human review based on community-specific rules.
* **Data Lookups:** Fetching and summarizing relevant data for users within specific gaming and tech communities.
* **24/7 Availability:** Running continuously to bridge the gap when human moderators are offline.

## 🛠️ Technical Implementation

This project utilizes the **PRAW (Python Reddit API Wrapper)** to interact with Reddit.

* **Language:** Python 3.10+
* **Dependencies:** `praw`, `pandas` (for data handling), `python-dotenv` (for security).
* **Compliance:** strictly adheres to Reddit's API terms of service.

## ⚖️ Rate Limiting & Compliance

This bot is engineered to be a "good citizen" of the Reddit API ecosystem:

1.  **Rate Limiting:** The bot strictly respects the standard API rate limit of **60 requests per minute**. It utilizes PRAW's built-in rate limit handlers to prevent spamming the API.
2.  **Opt-Out:** A clear opt-out mechanism is being implemented, allowing users to prevent the bot from interacting with their content.
3.  **User-Agent:** Uses a descriptive User-Agent string to identify itself transparently to Reddit's servers.

## 📦 Installation (Development)

*Note: This project is currently in the local development phase.*

1.  Clone the repository:
    ```bash
    git clone [https://github.com/yadu0124/redditAuto.git](https://github.com/yadu0124/redditAuto.git)
    ```
2.  Install dependencies:
    ```bash
    pip install -r requirements.txt
    ```
3.  Set up environment variables in a `.env` file:
    ```env
    CLIENT_ID=your_client_id
    CLIENT_SECRET=your_client_secret
    USER_AGENT=your_user_agent
    ```

## 📝 License

[MIT](LICENSE)
