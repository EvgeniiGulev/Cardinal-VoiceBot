
# Cardinal Voice Bot

Cardinal Voice Bot is a Discord bot that joins voice channels, listens for voice commands, and uses OpenAI's API to process and respond to commands.

---

## Features

- Joins a voice channel in your Discord server.
- Listens for voice commands from users.
- Sends recognized commands to OpenAI's API for processing.
- Responds with helpful outputs based on your input.

---

## Installation

Follow these steps to set up and run the bot:

### 1. Clone the Repository
Clone the bot's code to your local system using:
```bash
git clone https://github.com/your-repo/cardinal-voice-bot.git
cd cardinal-voice-bot
```

### 2. Install Dependencies
Install the necessary Nodejs packages:
```bash
npm install
```

### 3. Create the Configuration File
Inside the bot's root directory, create a folder named `config` and a file named `config.json` inside it.

```bash
mkdir config
nano config/config.json
```

Add the following to your `config.json`:
```json
{
  "token": "YOUR_DISCORD_BOT_TOKEN_HERE",
  "OPENAI_API_KEY": "YOUR_OPENAI_API_KEY_HERE"
}
```

Replace `YOUR_DISCORD_BOT_TOKEN_HERE` with your Discord bot token and `YOUR_OPENAI_API_KEY_HERE` with your OpenAI API key.

---

## Usage

### 1. Start the Bot
Run the bot using:
```bash
npm start
```

### 2. Invite the Bot to Your Server
1. Visit the [Discord Developer Portal](https://discord.com/developers/applications).
2. Select your bot and copy the "Client ID".
3. Use this URL to invite the bot:
   ```
   https://discord.com/oauth2/authorize?client_id=YOUR_CLIENT_ID_HERE&permissions=3147776&scope=bot
   ```
   Replace `YOUR_CLIENT_ID_HERE` with your bot's client ID.

### 3. Commands
- Join a voice channel: Use a command like `!join` (or customize the bot's join logic in the code).
- Speak commands, and the bot will process and respond.

---

## Notes

- Ensure your bot has permission to join voice channels and speak in them.
- If you plan to expand functionality, uncomment other API keys (Azure, etc.) in `config.json`.

---

## Troubleshooting

### Common Issues
- **Bot not responding:** Ensure your bot token and OpenAI API key are correct.
- **Dependencies missing:** Run `pip install -r requirements.txt` to ensure all required packages are installed.

### Logs
- Use logs in the terminal to debug issues and monitor activity.

---

## Contributing

Feel free to submit issues or pull requests on the GitHub repository.

---

## License

This project is licensed under the MIT License.
