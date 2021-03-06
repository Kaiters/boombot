#BOOM BOT V2.2.5

[![Build Status](https://secure.travis-ci.org/TerrordactylDesigns/boombot.png)](http://travis-ci.org/TerrordactylDesigns/boombot)

A bot for turntable.fm
Control a Queue,
Dj, welcome users,
tweet songs playing,
moderator chat, Last.fm,
Call out haters, etc
[Come play with one!](https://github.com/TerrordactylDesigns/boombot/wiki/Rooms-using-Boombot!-Add-yours!)

##Requirements

  Node.js
  NPM

##Optional Requirements

  Twitter API account
  Last.fm API account

##Basic Setup

* install Node.js and NPM

* Use your command shell of choice to get to the folder you want to install too.

* npm install boombot

* Drill to the node_modules/boombot folder and follow the below instructions

Create a FB or twitter account for your new bot.
Log in as the bot and use this to get your bots uid, auth token, and your rooms id:
http://alaingilbert.github.com/Turntable-API/bookmarklet.html
Now use the same method to get your personal accounts user id for control of the bot

Rename example.config.json to config.json and open in Sublime text 2 (Or your editor of choice... but really... go get sublime... its great..)
replace the xxxxxxxxxxxxxxxxxxxxxxxx's in the botinfo section with your bots auth, bot id, and replace the xxxxxxxxxxxx's in the admin section your own personal user id.
replace botname in the botinfo section with what you want to call the bot.

Download [Boombots Scripts](https://github.com/TerrordactylDesigns/Boombot-Scripts) and copy the ones you want into the scripts folder.

All that done? Ready for the magic?

    npm start

##Advanced Setup

Twitter - Get a Twitter API account and fill in the proper keys in the config file. Set tweet to true, fill in your rooms URL, the bot will now tweet the current playing song and a link to your room.

Last.fm - Get a Last.fm API account for the bot and fill in the proper keys in the config file. Set use to true, you will now have access to artist and song information. Set scrobble to true to scrobble room tracks to last.fm.

##Commands

Commands can be entered in chat or via PM to the bot

##Base Commands

* /lyrics - return the current playing songs lyrics

* /video - return the current playing songs video

* /help - lists the current bots commands

* /rules - returns the rules listed in the bots config.json file

* /boombot - returns the bots version and links to get your own

* /version - returns the bots current version

* /mods - the bot will list the current mods online in the room

* /theme - see the rooms current theme

###Base Commands When Last.fm Support Is Enabled And Configured

* /album - return the album the current song is from

* /similarsongs - return 3 similar songs to the current one

* /similarartists - return 3 similar artists to the current one

* /artistinfo - return information about the current artist playing

##Administrator/"The Master":

  All commands for the master require the setting for botname to trigger.
  Commands are not required to be in any order: example - This is a really good song boombot. Will trigger the 'boombot good' command. (replace boombot with whatever you set in the config.json)

* say - says in chat whatever you tell him to through pm

* djmode - make the bot get on stage and DJ

* getdown - make the bot get off stage

* skip - makes the bot skip the track it is playing

* good - remind the bot he's a good boy. Maybe he will kill you last during the robot apocalypse

* dance - make the bot upvote **this feature is not allowed and is de-activated by default**

* voodoo up - switch to the voodoo doll avatar (requires 100 dj points)

* kitten up - switch to the green kitten avatar (requires 300 dj points)

* alien up - switch to the alien avatar (requires 100 dj points)

* vampire up - switch to the vampire avatar (requires 100 dj points)

* avatar <number> - change the bots avatar to a specific one

* addsong - adds the current playing song to the bots playlist

* phone up - set the bots laptop to iPhone

* fruit up - set the bots laptop to Mac

* nix up - set the bots laptop to Linux

* chrome up - sets the bots laptop to ChromeOS

* droid up - sets the bots laptop to Android phone

* blacklist <username> - bans user from the room

* listbans - lists banned users, the mod who banned them, and when they were banned

* uptime - the bot returns its current uptime

##Queue commands

* /q - gives information on the current queue settings

* q - list the current queue

* q+ - add yourself to the queue

* q- - remove yourself from the queue

* /plays - list the play counts of each DJ on stage

##Queue control (Room Mods Only)

* /q on - turn the queue on

* /q off - turn the queue off

* /settings - see the queues current settings

* /1 - set the song limit to 1

* /2 - set the song limit to 2

* /3 - set the song limit to 3

* /none - set the song limit to 100

* vip <username> - move the user to the front of the queue

##Mod Commands

* /settheme <theme> - set the rooms current theme

* /notheme - shut off the rooms theme

##Mod Chat

Room moderators can PM the bot and it will PM the rest of the mods like a private chat room

##Automatic DJ mode

Boom Bot will hop up to save the day if the room drops to just 1 active DJ. He will hop back down again when a second DJ takes the stage.

##Tests

  npm test

##Notes

I know nothing about node. This was a playground that seemed to be liked. No warranties, no guarantees. I will however help you to the best that I can if you have any issues or find any bugs.

If you're more experienced than I am and want to tell me how to make this better in any way. I am all ears. Feel free to fork, if you come up with some cool scripts you can request a pull back and I will add them.

Lastly, ENJOY IT!!!!! It's not the best or most feature filled bot, but I appreciate you using him!
See the original and most feature filled version of Boom Bot at [Whistle while you work](http://turntable.fm/whistle_while_you_work43) where he lives.
