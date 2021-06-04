# Self-hosting - Discord welcome bot

[license]: https://github.com/Welcome-bot/welcome-bot/blob/main/LICENSE

Some of you may want to self-host the bot on your own VPS/server.  
This page explains how you can self-host the bot for yourself.

*Important!*
**By selfhosting the bot will you agree to the following terms:**
- You follow the [LGPL-v2.1-License][license] of the bot.
    - This means that you give credit to the original author (Welcome-bot team) and won't claim this code as your own.
- You aknowledge and agree that you won't receive any support for your self-hosted bot.

## Requirements
Before you can run the bot will you need to make sure that the following requirements are met.

### MongoDB
You need to have [MongoDB](//mongodb.com) installed and running on your server, where the bot will later run.  
This also includes creating databases and tables to later set in the `.env`.

### Node
You need **at least** Node 12 to be installed and working. Newer versions of Node should work too.

### Clone the repository
Clone the welcome-bot repository (Run `git clone https://github.com/Welcome-bot/welcome-bot`), if you didn't already and open it in your preferred IDE.

### .env
The `.env` is the environment vars of the bot in which you set various different information that will be used by the bot.  
To create it, first copy `.env.example` as `.env`, then add your bot token

Note that you don't have to set values for every option in the config.json.  
If you followed the previous step on preparing the bot will you only need to set the following options:

| Option:                | Value required:                                                     |
| ---------------------- | ------------------------------------------------------------------- |
| `BOT_TOKEN`            | Valid Bot-token of your Bot-application to login.                   |
| `MONGODB_URL`          | Valid URL provided by MongoDB when creating DB.                     |