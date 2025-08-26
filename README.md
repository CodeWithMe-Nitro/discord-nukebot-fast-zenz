# discord-nukebot-fast-zenz
a simply fast discord bot!

#📬 Discord Zenz MassDm / DM Bot
This is a Discord bot built using discord.py that allows server administrators to send direct messages (DMs) to individual users or all server members (excluding bots). It also supports retrying failed DMs and provides logging and status tracking.

⚙️ Features
!dm @user [message] Send a DM to a specific user.

!dmall [message] Mass DM all members in the server (except bots). Cooldowns included to reduce risk of rate-limits.

!dmretry <success_log_file> Retry sending DMs to users who were not successfully DMd previously.

!dmstatus Show a report of how many DMs were successfully sent and failed, based on the most recent log files.

🧠 Aliases
Command	Aliases
!dmall	!massdm, !dmallusers
!dmretry	!dmallcontinue, !retrydm, !dmfailures
📁 Log Files
When running mass DM campaigns, the bot will generate two log files:

✅ dm_success_<timestamp>.txt – list of users who received the message.

❌ dm_failed_<timestamp>.txt – list of users who failed to receive the message.

Retry logs are similarly named with dm_retry_success_<timestamp> and dm_retry_failed_<timestamp>.

🔐 Permissions
Only users with the Administrator permission can run DM commands.

🛠 Configuration
Edit the config.json file before running the bot:

{
  "token": "YOUR_BOT_TOKEN_HERE",
  "prefix": "!",
  "default_message": "This is a default DM message."
}
🚀 Running the Bot
Make sure you have Python 3.8+ and discord.py installed.

pip install -U discord.py
python bot.py
⚠️ Warnings
Abuse of mass DMing can get your bot or server banned. Use responsibly.

Cooldowns are in place (5 min every 20 users), but Discord can still rate-limit or flag spammy behavior.

🆘 Support & Contributions
Need help or have suggestions? You can reach out through these methods:

Discord: You can find me on Discord: xrszav
Telegram: You can also contact me on Telegram, @xrszav t.me/xrszav.
GitHub: If you have suggestions or improvements, feel free to open an issue or submit a pull request.
📄 License
This project is licensed under the MIT License. This project is provided as-is. You are responsible for how you use it.

🔑 Keywords
Discord Bot, Mass DM, Direct Messages, Bulk Messaging, Bot Development, Python, Discord.py, Admin Tools
