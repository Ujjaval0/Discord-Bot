# Discord-Bot

A Python-based Discord bot with various moderation, utility, and interactive commands.

## Features

*   **Welcome Messages**: Greets new members when they join the server.
*   **Content Moderation**: Automatically deletes messages containing specific keywords (e.g., "shit") and warns the user.
*   **Role Management**:
    *   `!assign`: Allows users to self-assign the "Gamer" role.
    *   `!remove`: Allows users to remove the "Gamer" role from themselves.
*   **Interactive Commands**:
    *   `!hello`: A simple command to check if the bot is responsive.
    *   `!dm <message>`: Echoes a message back to the user via DM.
    *   `!reply`: Replies directly to a user's command.
    *   `!poll <question>`: Creates a new poll with a custom question and pre-set reaction options.
*   **Role-Restricted Commands**:
    *   `!secret`: A command accessible only to users with the "Gamer" role.
*   **Logging**: Bot activities and errors are logged to `discord.log`.

## Technologies Used

*   **Language**: Python
*   **Library**: `discord.py` (for Discord API interaction)
*   **Configuration**: `python-dotenv` (for managing environment variables like the bot token)


## Bot Commands

*   `!hello` - Bot says hello.
*   `!assign` - Assigns the "Gamer" role to you.
*   `!remove` - Removes the "Gamer" role from you.
*   `!dm <your message>` - The bot DMs you back with `<your message>`.
*   `!reply` - Bot replies to your command message.
*   `!poll <Your Poll Question>` - Creates a poll with 👍, ❤️, 🙌, 👎, 🤣 reactions.
*   `!secret` - (Requires "Gamer" role) Sends a secret message.

## Project Structure

```
Discord2/
├── .env           # Environment variables (contains DISCORD_TOKEN) - **DO NOT COMMIT THIS FILE**
├── .venv/         # Python virtual environment
├── main.py        # Main application script for the bot
├── requirements.txt # Python dependencies
└── discord.log    # Log file for bot activity
```
