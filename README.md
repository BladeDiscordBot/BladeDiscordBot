# BladeDiscordBot
A Discord self-bot with multipurpose/server nuking features.

This version of the bot is free for you to use, distribute, etc. You may pay to receive the premium version by e-mailing me at bladediscordbot@gmail.com. It only costs $10 and will guarantee you updates for the life of the project.

# Recent Updates
- Bot now deletes command after it is run.
- Bot now recognizes when you are banned/lose permissions in a server, and stops command if this is the case as opposed to having to restart the bot every time.
- New command for premium users - !masspingall.

# Setup
Install Python 3.6.6 and in the setup process, ensure you check off "Add Python to PATH" if you are running on Windows. Install discord.py using pip install discord.py. Input your user token into the source code where it says "token". You may adjust the prefix (the symbol you must type before every commmand) and the yprefix (prefix for YAGPDB.xyz bot, if your target server relies on moderation  through that bot) to your liking. That's it! The bot should run after that. Send me an e-mail if you have any problems, or create an issue on this GitHub page.

# Tips
If the bot says "you may have been banned", "breaking out of method", or something along these lines, it means that you have either been banned from the targeted server, or you don't have permission in the server to run the command selected.

Some commands may have a random delay. This is because the Discord API only allows a user to make so many requests at once. Most commands don't suffer as a result of this, except for !autoname, !namestealer, !pingall and !masspingall, but the delay is minimal nonetheless.

If you cannot run the script due to some sort of error, please contact me using my e-mail bladediscordbot@gmail.com.

# Free Commands
These commands can be run by cloning this repository and running the Python script.

## autoname
Changes your nickname in targeted server to a random string of characters ranging from 2-32 character length every second.
## newname
Changes your nickname in targeted server to a random string of characters ranging from 2-32 character length once.
## kickall
Allows you to kick all members in the server if you have the permission to do so.
## banall
Allows you to ban all members in the server if you have the permission to do so.
## ykickall
Allows you to kick all members in the server using the YAGPDB.xyz bot. Useful if server is configured in such a way that all moderation goes through this bot.
## ybanall
Allows you to ban all members in the server using the YAGPDB.xyz bot. Useful if server is configured in such a way that all moderation goes through this bot.
## ping
Pings a random member of the server and instantly deletes it.
## faketyping
Simulates a typing status in targeted channel. Lasts until you are banned from the server or exit the bot.
## stop
Disconnects the bot, stops all commands, and quits the application.

# Premium Commands
You must purchase the bot to use these commands. Contact me at bladediscordbot@gmail.com if you are interested.

## namestealer
Changes your nickname in targeted server to another member's username every second. Lasts until you are banned from the server or leave.

## pingall (optional arg "delay")
Constantly pings all members of the server, one by one, instantly deleting each message. Lasts until you are banned from the server or leave.

## masspingall (NEW) (optional arg "delay")
Fits as many member's mentions as it can into one message, sends the message and instantly deletes it. Keeps sending these messages until you are banned or leave the server.

## faketypingall
Simulates user typing in all available channels. Discord API prevents too many calls to this, so this command is a little inconsistent, but still very effective.

## spamwipe
Wipes all channels, roles, emojis and members from the server, if you have the appropriate permissions. If the wipe completes before being banned, it also adds bogus channels and roles to make server cleanup more difficult.

## wipe
Deletes all emotes, channels, and roles in targeted server, if you have the appropriate permissions.

## spamserver
Adds a bunch of garbage channels and roles to targeted server, if you have the appropriate permissions.

## nowplaying (required arg "game")
Simulates playing a game on Discord. Takes one argument with the game's name. (Example call: nowplaying games)

## spamtext (optional arg "delay")
Spams all messages written in companion "text_to_spam.txt" file that comes with the bot to targeted channel. Lasts until you are banned from the server or exit the bot.

# Arguments

# delay
Amount of time, in seconds, to delay the command from running itself again.

# game
The name of the game you want to simulate playing on Discord.
