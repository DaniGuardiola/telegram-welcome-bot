[![js-standard-style](https://cdn.rawgit.com/feross/standard/master/badge.svg)](https://github.com/feross/standard)

# Telegram Welcome Bot

Simple Telegram bot that sends a welcome message to new members
Created by Dani Guardiola

# Features

- Welcomes new members to a group
- Message can be changed with the `/change_welcome_message` command
- Filesystem persistence for restart resilience
- Dead-easy deployment and setup

# Installation

> You need NodeJS v8+ installed on your server to deploy and run this bot

1. Clone this repo on a server
2. Execute `npm i` on the repo directory
3. Create a bot through the [@BotFather](http://t.me/botfather) bot to obtain both a `bot api token` and a `bot username` (`@example_bot`)
4. Execute `npm run start -- --persistence-path <path for persistence> --api-token <your bot's token> --bot-username <your bot's username>`

> Command line options have the following short forms:
> - `--persistence-path`: `-p` (default path is `<repo directory>/.persistence`)
> - `--api-token`: `-t`
> - `--bot-username`: `-u`

## Command list

For autocompletion and command list within the Telegram apps, you might want to configure the command list through BotFather.

For your convenience, here's a copy-paste list of the commands, correctly formatted:

```
change_welcome_message - Changes the welcome message of the group
help - Displays a help message
```

# Example

```
$ npm run start -- -p ~/bot -t 582659278:JsjjSHDNns-JjshJhann2nhJjans88kKSiw -u welcome_message_bot
```

Enjoy!
