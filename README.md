# Telegram Personal Assistant Bot

![GitHub license](https://img.shields.io/badge/license-MIT-blue.svg)

This is a Telegram bot written in Golang that serves as a personal assistant. It leverages the [Telegram Bot API](https://core.telegram.org/bots/api) for communication with users and the [OpenAI GPT-3.5 Turbo](https://beta.openai.com/docs/introduction/gpt-3) for generating responses.

## Features

- Responds to user messages and commands.
- Implements basic commands like `/help`, `/sayhi`, and `/status`.
- Can generate intelligent responses using GPT-3.5 Turbo for any user input.

## Getting Started

Firstly, need to provide an `OPENAI_TOKEN` and `TELEGRAM_TOKEN` as an  enviroment variables

### Prerequisites

- Go installed on your system.
- Telegram bot token obtained from the BotFather on Telegram. Put it to `TELEGRAM_TOKEN` env variable.
- OpenAI API key. Put it to `OPENAI_TOKEN` env variable.

### Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/your-username/telegram-personal-assistant-bot.git
   ```

2. Install dependencies:

   ```bash
   go get github.com/go-telegram-bot-api/telegram-bot-api/v5
   go get github.com/sashabaranov/go-openai
   ```

3. Update the bot token and OpenAI API key in the `main.go` file.

4. Build and run the bot:

   ```bash
   go build
   ./your-bot-executable
   ```

### Usage

1. Start a chat with your bot on Telegram.

2. Send messages to the bot, and it will respond to your messages using OpenAI's GPT-3.5 Turbo for intelligent responses.

3. You can also use the following commands:
   - `/help`: Get information about available commands.
   - `/sayhi`: Get a friendly greeting from the bot.
   - `/status`: Check the bot's status.

### Customization

You can customize the bot's responses, add more commands, and adapt its behavior as needed by modifying the `main.go` file. For more advanced interactions with GPT-3.5 Turbo, refer to the [OpenAI API documentation](https://beta.openai.com/docs/introduction/gpt-3).

### License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

### Acknowledgments

- [Telegram Bot API](https://core.telegram.org/bots/api)
- [OpenAI GPT-3.5 Turbo](https://beta.openai.com/docs/introduction/gpt-3)
