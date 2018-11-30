# SWGOH Payout Countdown Discord Bot

![screenshot](/botscreenshot.png)

# Prerequisites

 - Admin rights on the target Discord server
 - A Facebook or [GitHub](https://github.com/) account for use with [Glitch](https://glitch.com/)
 - An [UptimeRobot](http://www.uptimerobot.com/) account

All these steps will need to be done on a computer.

# Setup

## Set up Discord

 - Browse to https://discordapp.com/developers/applications/
 - Click "Create an application"
 - (You can set an icon and give the project a name, but it doesn’t really matter. What you set here won’t appear anywhere besides the Discord application list.)
 - Click "Copy" under "Client ID". Paste the Client ID somewhere. You'll need it later.
 - Select "Bot" under "Settings"
 - Click "Add Bot"
 - This is where you set the bot's name and icon
 - Once you've done that, click "Copy" under "Token". Make sure you paste this somewhere for later too.
 - Replace the zeros in this URL with the Client ID you copied before: https://discordapp.com/api/oauth2/authorize?client_id=000000000000000000&scope=bot&permissions=8
 - Visit your edited URL and you'll be prompted to choose which server the bot should join.
 - Browse to the channel you want the bot to operate in and copy the last  part of the URL. The numbers after the last slash are the Channel ID. (For example, in https://discordapp.com/channels/000000000000000000/111111111111111111 the Channel ID is 111111111111111111.)

## Set up Glitch

 - Browse to https://glitch.com/edit/#!/payout-countdown
 - Click "Remix This" in the upper-right corner
 - Click the project name in the upper-left and choose "Sign In"
 - Once you're signed in, click the project name again and click the lock icon underneath. This makes your project private.
 - Select the 🗝.env file in the list on the left.
 - Paste the Channel ID you copied after "writeChannelId="
 - Paste the Token you copied earlier after "botToken="
 - Select the shard-data.json file on the left. This is where your user data is stored. Make sure you use a valid swgoh.gg URL for each user.
 - Once you're done editing the shard-data.json, click "Logs" on the left, then click "Console" down below. 
 - A new tab will open with the Glitch console. Type "refresh" and hit enter. The application will restart and you should see your changes reflected on the bot in a minute or two.
 - Go back to the project page and click "🕶 Show" at the top. This will open a new tab that will just say "OK". Copy this page's URL for the next section.

## Set up UptimeRobot

 - Log in to https://uptimerobot.com/
 - Browse to the Dashboard
 - Click "+ Add New Monitor"
 - Choose "HTTP(S)" for monitor type, give it a name, and paste the URL you just copied in the "URL (or IP)" field.
 - Make sure the interval slider is set to 5 minutes.
 - Click "Create Monitor".

You can rename the current file by clicking the file name in the navigation bar or by clicking the **Rename** button in the file explorer.

## Credits
Original bot written by [Tarnadas](https://github.com/Tarnadas/shard-payout) [(Reddit thread)](https://www.reddit.com/r/SWGalaxyOfHeroes/comments/71904d/i_made_a_discord_bot_for_our_shard_to_track_time/)

## Contact

Feel free to contact me on Discord: @nerfherder42#4397 
