# Family Tree Game Bot

This project is a Telegram bot for a Family Tree Game, built using Python and the python-telegram-bot library. It includes a database schema for storing user data, image generators for family tree visualization, and Docker configuration to streamline deployment.

## Project Structure
.
├── bot/
│   ├── __init__.py
│   ├── bot.py
│   ├── handlers/
│   │   ├── __init__.py
│   │   ├── command_handlers.py
│   │   ├── message_handlers.py
│   │   └── callback_handlers.py
│   └── utils/
│       ├── __init__.py
│       ├── database.py
│       ├── image_generator.py
│       └── config.py
├── db/
│   └── schema.sql
├── docker/
│   ├── Dockerfile
│   └── docker-compose.yml
├── tests/
│   ├── test_bot.py
│   └── test_database.py
├── requirements.txt
└── README.md

## Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/sohamsingh419/fam-bot.git
   cd fam-bot
   ```
2. Install the dependencies:
   ```bash
   pip install -r requirements.txt
   ```

3. Set up the database schema:
   ```bash
   sqlite3 db/schema.sql < db/schema.sql
   ```

4. Run the bot:
   ```bash
   python bot/bot.py
   ```

## Docker
To run the bot using Docker, use the following command:
```bash
docker-compose up
```
