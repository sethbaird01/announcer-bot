# announcer-bot
A discord bot for making server-wide announcements. 

# Important: READ
This project is not done, and I don't recommend adding this to your server until further improvements and refinements are added. Feel free to contribute, but honestly I would recommend just going with a fully finished bot for the time being. I'm creating this bot as a personal project and to test my skills with discord.js

## Contributors:
This is my first fully public repo, and as such I'm not experienced with managing a group project with github. If there's anything I'm missing in terms of project management or team development plesae let me know so I can change it asap.

For feature management, I integrated a project board with my goals for this bot. 

## Planned featureset

Persons allowed to make announcements are defined as "approved" in the below list.

* To become approved, the inviter of the bot or a mod of the server must issue a command to the bot stating so.
* To make an announcement, an approved server member must first DM the bot a link and title for the announcement, then after that, the bot will reply with a list of images in the website. Once an image is selected, the embed will be created contained LINK, IMAGE, and TITLE. This embed will be sent back to the requestor where they can then approve or deny the broadcast. Approving will submit the newly created embed.
* Note: If the user making an announcement is in multiple serves with the bot, they will be requested to choose a server/servers for the announcement to be sent to.
* Before the announcement is sent, a target channel must be set for every server. Usually, this will be done before the first announcement can be set. For example: upon inviting the bot to a server (or getting approved), the user will recieve DM showing each server, and request a channel for announcements to be sent to. This "announcements channel" will be stored in the bot's database per-user.
* If the announcement doesn't include a link, the bot will generate a standard embed with no image or link.
