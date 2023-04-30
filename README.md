# Activity Archivist (issues)
1. You can report issues and bugs regarding **Activity Archivist#4042**, or suggest new features if you want to.<br/>
2. Before posting a new issue, please check if already exists.
###### (give me as many details as you can, so I can help you faster)

- ***Quick note: The bot only updates your playtime when your status message is changed. (eg. when you exit the game)***
<br/><br/><br/>

## Basic commands to help you get started:

### Help
#### /help [submenu]
This command displays the help menu. You can use it like this */help* or like this */help [submenu]*. If you want to see more about a specific command use the second option. (eg. */help track*)

### Track
#### /track {user}
This command creates a profile for the mentioned user (You can use */track @yourusername* to register yourself or */track @otherusername* to register someone else).
The bot only saves a user's activities (playtimes) if they're registered. Don't worry, registering is easy: just use the */track* command. That's it.

### Stats
#### /stats [user]
This command is used to read the saved playtimes. You can use */stats* to fetch your own stats or use the */stats @username* to read someone else's stats.<br/>
**Important things to know:**
- you can only use this command on registered users (read */track* for more info)
- if you don't want others to use */track @yourname*, you can block them (read */block-tracking* for more info)

### Block tracking
#### /block-tracking [block] [user]
This command is a bit hard to understand, but once you get it, it's not that complicated.<br/>
This command can be used for 2 different things:
**(1)** 'un-register' yourself (pauses status message recording)
**(2)** block a specific user (so they can't use */stats @yourusername*)

There are 2 optional arguments as well (the *block* and the *user*).
- The *block* argument:
- - it has 2 value (*Block* or *Allow*)
- - if you don't specify it, it will use its default value (which is *Block*)
- The *user* argument:
- - if you don't put anything in there => **(1)**
- - if you put specify a user, that user will be blocked or unblocked only => **(2)**

Some examples:
- */block-tracking @example123*
- - only blocks @example123 (you can use */block-tracking @Barni#6264 Block* too)
- */block-tracking*
- - pauses playtime recording and */stats @yourusername* for everyone (you can also use */block-tracking Block*)
- */block-tracking Allow*
- - 're-registers' (opposite of */block-tracking* and */block-tracking Block*)

### Delete data
#### /delete-data 'DELETE'
This command permanently removes all saved playtime stats.<br/>
Note: */delete-data* does not disable tracking and does not unregister you. (read */block-tracking* for more info)

### About
#### /about
About me page and info

### Autostat
#### /autostat
Automatically sends stats in the DM channel every 24 hours.
You can toggle autostat on or off with this command if you're a supporter. Every day at 10:00 PM (22:00) GMT/UTC you get a message that contains your pie chart (like the one you get when you use /stats)

### Support
#### /support
Maintaining and running a bot 24/7 can be expensive and time-consuming. If you want to help, you can report issues and bugs on Github, or you can make a donation to support the development and operation of the bot
