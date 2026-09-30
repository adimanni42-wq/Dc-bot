# Discord Slash Bot

Ready for GitHub + Railway.

## 1. Create the Discord bot
Discord Developer Portal → New Application → Bot → Reset Token.
Also copy the Application ID (Client ID).

## 2. Upload this folder to GitHub
Upload:
- index.js
- package.json
- .env.example
- README.md

Do NOT upload your real token.

## 3. Railway
Create a project from your GitHub repository.
Start command:
`npm start`

Add Variables:
- DISCORD_TOKEN = your bot token
- CLIENT_ID = your Application ID
- GUILD_ID = your server ID (recommended while testing)

## 4. Invite the bot
Create an OAuth2 URL with scopes:
- bot
- applications.commands

Give only the permissions your bot actually needs. Moderation commands need the matching Discord permissions.

## Commands
The bot registers the slash versions of the commands from your screenshots, including:
General, Staff, Server, Tickets, Economy, Moderation, Channel, Announce, Games, Levels, Info and Giveaway.

Important: several advanced commands are included as working command endpoints but are intentionally simple placeholders until you connect a database/configuration for your server.
